# 中級 問題05: querySelector で DOM 取得

**難易度: ★★★★☆☆☆☆☆☆**

## 🎯 やること

JavaScript で HTML 要素を**取得してテキストを書き換える**基本を学びます。

## ✅ 要件

`script.js` に以下を書いてください。

1. `document.querySelector('#title')` で `<h1>` を取得し、テキストを `"書き換えられました！"` に変更する
2. `document.querySelector('.description')` で段落を取得し、テキストを `"JavaScript で DOM を書き換えた結果です。"` に変更する
3. `document.querySelectorAll('.item')` で全ての `.item` を取得し、 それぞれの中身に 順に `"A"`, `"B"`, `"C"` と書き込む

## 👀 確認方法

- ページを開くと h1 の文字が変わっている
- p の文字も変わっている
- 3つの `.item` の中身が A / B / C に置き換わっている

## 💡 ヒント

```js
const el = document.querySelector('#title');
el.textContent = '新しい文字';
```

- `querySelector` → **最初の1つ**を返す（CSS セレクタが使える）
- `querySelectorAll` → **すべて**を NodeList で返す（`forEach` で回せる）
