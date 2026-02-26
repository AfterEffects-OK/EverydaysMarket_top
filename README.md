# Everyday's Market Website

これは、Webデザインの講義・演習用に作成された架空のライフスタイル提案型ミニスーパー「Everyday's Market」のウェブサイトです。

## 概要

このプロジェクトは、HTMLとCSS（Tailwind CSSフレームワークを含む）を使用して構築された、静的なウェブサイトです。モダンでクリーンなデザインを目指し、以下のページで構成されています。

*   **トップページ (`index.html`)**: 店舗のコンセプト、おすすめ商品、生産者の紹介、アクセスマップなど、ウェブサイトのメインとなるコンテンツ。
*   **採用情報ページ (`recruit.html`)**: 募集職種の一覧や、求める人物像などを掲載。
*   **エントリーページ (`entry.html`)**: 採用への応募ページ（現在は受付終了のダミー表示）。

## 特徴

*   **Tailwind CSS**: ユーティリティファーストのCSSフレームワークを利用し、迅速なUI開発を実現。
*   **レスポンシブデザイン**: スマートフォンからデスクトップまで、様々なデバイスで快適に閲覧可能。
*   **CSSの外部ファイル化**: `style.css`に共通のスタイルを分離し、保守性と再利用性を向上。
*   **Webフォント**: `Google Fonts` (`Noto Sans JP`, `Shippori Mincho`) を利用し、豊かなタイポグラフィを表現。
*   **アイコン**: `Font Awesome` を利用し、視覚的に分かりやすいUIを実装。

## 使用技術

*   HTML5
*   CSS3
*   Tailwind CSS
*   Font Awesome
*   Google Fonts

## 技術仕様

### 1. ディレクトリ構成

```
.
├── index.html      (トップページ)
├── recruit.html    (採用情報ページ)
├── entry.html      (エントリーページ)
├── style.css       (共通スタイルシート)
└── README.md       (このファイル)
```

### 2. CSS設計

*   **Tailwind CSS**: 基本的なスタイリングとレイアウトは、CDN経由で読み込まれるTailwind CSSのユーティリティクラスを使用しています。
*   **`style.css`**: サイト全体で共通のカスタムスタイル（Webフォントの定義、ブランドカラー、`nav-link`のアニメーションなど）を定義しています。
*   **カスタムプロパティ (CSS Variables)**: `:root` でブランドカラーなどを変数として定義し、一貫性のあるデザインとメンテナンス性の向上を図っています。

### 3. レスポンシブ対応

Tailwind CSSのブレークポイント (`sm`, `md`, `lg`など) を利用して、モバイルファーストで実装されています。ナビゲーションメニューは `md` 以上の画面で表示され、それ以下のサイズでは非表示になります（ハンバーガーメニューは未実装です）。

### 4. 外部ライブラリ

本プロジェクトでは、以下のライブラリをCDN経由で利用しています。
*   **Tailwind CSS**: `https://cdn.tailwindcss.com`
*   **Font Awesome**: `https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css`
*   **Google Fonts**: `https://fonts.googleapis.com/` (`Noto Sans JP`, `Shippori Mincho`)

## サイトの閲覧方法

各`.html`ファイル（`index.html`, `recruit.html`, `entry.html`）を直接ウェブブラウザで開くことで閲覧できます。

## 注意事項

このウェブサイトは学習目的で作成されたサンプル（ダミー）です。記載されている店舗、サービス、採用情報はすべて架空のものであり、実在の団体とは一切関係ありません。
