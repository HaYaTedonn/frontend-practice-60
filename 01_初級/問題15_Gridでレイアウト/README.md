# 初級 問題15: Grid でレイアウト

**難易度: ★★★★☆☆☆☆☆☆**

## 🎯 やること

`display: grid` で、**3列3行のグリッド**を作ってみましょう。

## ✅ 要件

1. `.grid` に次を指定
   - `display: grid;`
   - 3 列（`grid-template-columns: 1fr 1fr 1fr`）
   - 行と列の隙間 `gap: 12px`
2. `.cell` に次を指定
   - 背景色: `mediumpurple`
   - 文字色: 白
   - 高さ: `80px`
   - 文字を縦横中央に置く（flex でもgrid でも OK）
   - 角丸: 6px

`.cell` は HTML に 9 個用意されています。

## 👀 確認方法

3×3 のマス目ができ、均等な幅で並ぶ。

## 💡 ヒント

- `1fr` は「残りの空間を均等に分ける単位」
- `grid-template-columns: repeat(3, 1fr)` とも書ける
