# Master Reference App

モダナイズ後のマスタ参照システム（サブシステム 01〜09）。
`doc/design/specs-tobe/` の設計に基づくブランクプロジェクト。

## 技術スタック

- Java 21
- Spring Boot 3.x (Web / Validation / JDBC / Actuator)
- PostgreSQL
- Flyway

## 対象サブシステム

- 01-calendar
- 02-branch
- 03-customer
- 04-customersearch
- 05-product
- 06-interestrate
- 07-feeschedule
- 08-account
- 09-accountlifecycle

## ビルド

```bash
mvn clean package
```

## 起動

```bash
mvn spring-boot:run
```

デフォルトポート: `8081`

## 環境変数

| 変数 | 既定値 | 説明 |
|---|---|---|
| `DB_URL` | `jdbc:postgresql://postgres:5432/banking` | DB接続URL |
| `DB_USER` | `cobol` | DBユーザー |
| `DB_PASSWORD` | `cobol` | DBパスワード |
| `SERVER_PORT` | `8081` | HTTPポート |
