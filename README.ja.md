# web-audio-piano

Web Audio API を利用した小さなピアノライブラリとデモ集です。

## 概要

- ライブラリ: `src/` に TypeScript 実装が含まれます。
- デモ: `apps/next-demo`（Next.js）と `apps/vite-demo`（Vite + React）があります。
- ドキュメント: `docs-site/` にドキュメントと VitePress 設定があります。

## 必要条件

- Node.js 20 以上

## クイックスタート

ルートで依存をインストールしてビルドします（CI と同じコマンド群）。

```bash
npm install
npm run build          # ライブラリ全体のビルド
npm run build:next     # Next.js デモのビルド
npm run build:vite     # Vite デモのビルド
npm run build:docs     # ドキュメントサイトのビルド
```

ローカルでデモを確認したい場合は、各アプリの `package.json` のスクリプトを確認して実行してください。例えば:

```bash
cd apps/next-demo
# スクリプトを確認
cat package.json | sed -n '1,200p'

cd ../vite-demo
# スクリプトを確認
cat package.json | sed -n '1,200p'
```

（各アプリは一般的に `dev` / `start` / `build` スクリプトを持っています。プロジェクト固有の実行方法は該当 `package.json` を参照してください。）

## 開発

- TypeScript ソースは `src/` にあります。型定義やユーティリティを修正したらルートで再ビルドしてください。
- VSCode を使う場合、`.vscode` 関連の設定は `.gitignore` で適切に管理されています。

## ディレクトリ構成（抜粋）

- `src/` - ライブラリ本体
- `apps/next-demo` - Next.js デモ
- `apps/vite-demo` - Vite + React デモ
- `docs-site/` - ドキュメントサイト（VitePress など）

## コントリビューション

1. Issue を立てるか、フォークして PR を送ってください。
2. 変更を加えたらテストとビルドをローカルで確認してください。

## ライセンス

（必要であればここにライセンス情報を追加してください）

---

この README は日本語での簡易案内です。英語の README（`README.md`）も併せて参照してください。
