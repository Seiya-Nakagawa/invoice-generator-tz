# 要件定義書

本ツールの要件定義は、ベースリポジトリのドキュメントを参照してください。

> **参照先**: [invoice-generator / docs/REQUIREMENTS.md](https://github.com/Seiya-Nakagawa/invoice-generator/blob/main/docs/REQUIREMENTS.md)

## TZ向け差分

本リポジトリは `invoice-generator` の処理をベースに、以下の設定のみ変更しています。

| 項目 | invoice-generator | invoice-generator-tz |
|------|-------------------|----------------------|
| Gmailラベル名 | `SJ_請求書テンプレート` | `TZ_請求書テンプレート` |
| `EMAIL_SUBJECT_TEMPLATE` | SJ向けの件名テンプレート | TZ向けの件名テンプレート |
