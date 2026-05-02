# 基本設計書

本ツールの基本設計は、ベースリポジトリのドキュメントを参照してください。

> **参照先**: [invoice-generator / docs/DESIGN.md](https://github.com/Seiya-Nakagawa/invoice-generator/blob/main/docs/DESIGN.md)

## TZ向け差分

本リポジトリは `invoice-generator` の処理をベースに、以下の設定のみ変更しています。

| 項目 | invoice-generator | invoice-generator-tz |
|------|-------------------|----------------------|
| Gmailラベル名 | `SJ_請求書テンプレート` | `TZ_請求書テンプレート` |
| `EMAIL_SUBJECT_TEMPLATE` | SJ向けの件名テンプレート | TZ向けの件名テンプレート |
