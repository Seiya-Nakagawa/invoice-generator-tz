# invoice-generator-tz

TZ向けの請求書PDF生成・Gmail下書き作成ツール（Google Apps Script）。

## 概要

Google スプレッドシートに紐付けた GAS として動作し、以下の処理を自動化します。

1. **当月シート作成**: フォーマットシートをコピーして当月分の請求書シートを作成
2. **PDF作成 & Gmail下書き**: 前月分のシートをPDF化し、Googleドライブに保存してGmail下書きを作成

## セットアップ

### 1. GASスクリプトプロパティの設定

| キー | 値の例 | 説明 |
|------|--------|------|
| `EMAIL_SUBJECT_TEMPLATE` | `【TZ】請求書_{YEAR}年{MONTH}月分` | メール件名・PDFファイル名のテンプレート |

### 2. Gmailラベルの設定

Gmail で `TZ_請求書テンプレート` というラベルを作成し、メール本文・宛先を設定した下書きに付与してください。

### 3. スプレッドシートの設定

- フォーマットシート名: `フォーマット`（`config.gs` の `FORMAT_SHEET_NAME` で変更可）

## 開発

```bash
# GASへの反映
clasp push -f
```
