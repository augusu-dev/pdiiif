# pdiiif

IIIF ManifestからPDFを生成するツールです。ブラウザ上で完結し、サーバー不要で動作します。

**Demo**: https://augusu-dev.github.io/pdiiif/

## Features

- IIIF ManifestのCanvasごとにPDFページを生成
- ALTO/hOCR OCRによる隠しテキストレイヤー
- IIIF RangeからのPDF目次
- IIIF AnnotationのPDF注釈としての描画
- Manifest・OCRファイルのPDF添付
- Polyglot PDF/ZIPの生成

## Supported IIIF Sources

URLをそのまま入力するだけで動作します。以下の形式に対応：

- IIIF Presentation API v2/v3 Manifest URL
- 国立国会図書館デジタルコレクション（`https://dl.ndl.go.jp/pid/{PID}`）※IIIF対応資料のみ

## Development

```
pnpm install
pnpm run -r build
```

## Repository Structure

- `pdiiif-lib/` — コアライブラリ (TypeScript)
- `pdiiif-api/` — Express APIサーバー (オプション)
- `pdiiif-web/` — Svelte Webアプリ

Forked from [jbaiter/pdiiif](https://github.com/jbaiter/pdiiif)
