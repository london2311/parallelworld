# パラレル対話盤 v3 — 三三三の揺らぎ・深層六声協議

ひらがな333音のランダムな揺らぎから、六つの「自分」の発言力を配分し、AIに貼り付けるための「開会の言葉」を生成する自己対話アプリです。

## 特徴

- 完全静的アプリ。APIキー不要。
- Vite + React 構成。
- 333音の生成と発言力ランキング。
- 浮上した言霊の検出。
- v3プロンプトで、各声に「代償」「反論」「隠れた前提」「禁止ワード」を追加。
- ChatGPT / Claude / Gemini などに貼り付けて使えます。

## ローカル起動

```bash
npm install
npm run dev
```

## ビルド

```bash
npm run build
```

## GitHub Pages に上げる場合

Vite の通常構成です。リポジトリ名配下で公開する場合は `vite.config.js` で `base` を設定してください。

例: リポジトリ名が `parallel-council-board` の場合

```js
import { defineConfig } from "vite";
import react from "@vitejs/plugin-react";

export default defineConfig({
  plugins: [react()],
  base: "/parallel-council-board/",
});
```
