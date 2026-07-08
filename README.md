# 柏の葉スマートシティ ゼミ研修提案プレゼンテーション

reveal.js を用いた大学ゼミの研修先提案スライドです。

## 概要

| 項目 | 内容 |
|------|------|
| テーマ | 柏の葉スマートシティ（千葉県柏市）をゼミ研修先として提案 |
| 発表時間 | 約3分 |
| スライド枚数 | 6枚 |
| 発表者 | 河合ゼミ4年 村松友哉 |

## スライド構成

1. **タイトル** — ゼミ研修候補地の提案（背景画像 + オーバーレイ）
2. **選定理由** — 4つのカードで選択理由を説明
3. **視察予定場所** — 画像付きカードで各施設を紹介
4. **行程** — タイムライン形式（1泊2日）
5. **予算** — インフォグラフィック形式で内訳 + 合計
6. **まとめ** — 3つの学びの柱 + 提案

## 技術スタック

- [reveal.js](https://revealjs.com/) v5.1.0（CDN）
- Vanilla CSS / JavaScript（カスタムテーマ）
- GitHub Pages に対応

## ファイル構成

```
.
├── index.html          # メインエントリポイント
├── css/
│   └── custom.css      # カスタムスタイル（moonテーマ上書き + 印刷対応）
├── js/
│   └── custom.js       # Reveal.initialize() 設定
├── img/                # 画像フォルダ（今回はUnsplash直リンクを使用）
└── README.md           # 本ファイル
```

## 使い方

### ローカルで開く

```bash
# ブラウザで直接開く
start index.html
```

### PDF 出力

Chrome で以下の URL にアクセスし、印刷（Ctrl+P）→「PDFに保存」を選択。

```
index.html?print-pdf
```

> `?print-pdf` パラメータを付与することで、レイアウト崩れなく PDF 出力できます。

### GitHub Pages で公開

1. このリポジトリを GitHub に Push
2. Settings → Pages → Source: `Deploy from a branch`
3. Branch: `main` / folder: `/ (root)` を選択
4. 数分後 `https://<ユーザー名>.github.io/<リポジトリ名>/` で公開完了

## カスタマイズ方法

### スライド内容の変更

`index.html` の各 `<section>` 内のテキストを編集してください。各スライドにはコメント付きで役割を記載しています。

### デザインの変更

- **配色**: `css/custom.css` の `:root` 内のカスタムプロパティを変更
- **テーマ**: `index.html` の `theme/moon.css` を `white.css` などに差し替え（その場合はカスタムCSSの調整が必要）

### 画像の差し替え

`index.html` 内の `<img>` タグの `src` を差し替えてください。`img/` フォルダに画像を配置し、相対パスで参照することも可能です。

## ライセンス

- プレゼンテーション内容: 自由にご利用ください
- Unsplash 画像: [Unsplash License](https://unsplash.com/license) に準拠
