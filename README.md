# AI Viz Frontend

> Next.js (App Router, TypeScript, Tailwind CSS) + Storybook + Vitest 構成のフロントエンドプロジェクト

---

## 🚀 セットアップ

```bash
# パッケージインストール
npm install
```

---

## 🧪 開発サーバー

```bash
npm run dev
```

- http://localhost:3000  
- `src/app` ディレクトリ構成を採用した **App Router** アーキテクチャです。

---

## 🧱 Storybook（UI コンポーネント開発）

```bash
npm run storybook
```

- http://localhost:6006  
- **Tailwind CSS は本番と同じスタイルで適用されます**  
- `src/components/**/*.stories.tsx` に Story ファイルを配置

---

## 🧹 Lint & Format

```bash
# コードチェック（ESLint）
npm run lint

# 自動整形（Prettier）
npm run format
```

---

## 🧪 テスト（ユニット）

```bash
npm run test
```

- **[Vitest](https://vitest.dev/)** による高速なユニットテスト
- 設定ファイルは `vitest.setup.ts` に定義

---

## 📁 ディレクトリ構成（抜粋）

```
src/
├── app/              # Next.js App Router 構成
├── components/       # UIコンポーネント群（Storybook対応）
├── lib/              # ロジック系の共通関数など
└── tests/            # テストコード
.storybook/
├── main.ts           # Storybook 設定
└── preview.ts        # Tailwind CSS の読み込みなど
```

---

## 🛠 使用技術・ツール

- **Next.js** 13+ App Router
- **TypeScript**
- **Tailwind CSS** v4 対応
- **PostCSS** + `@tailwindcss/postcss`
- **Storybook** 7.x（Vite + Next.js 対応）
- **Vitest**（Jestライクな高速テストランナー）
- **ESLint / Prettier**

---

---

## 📝 コントリビュート

1. `dev/frontend` フロントエンド開発用メインdevブランチ
2. `feat/frontend/***`, `fix/frontend/***`, `chore/frontend/***` など GitHub Flow に準拠
3. `dev/frontend` へプルリクエスト