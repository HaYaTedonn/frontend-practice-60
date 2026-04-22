# 中級 問題07: classList でクラス操作

**難易度: ★★★★★☆☆☆☆☆**

## 🎯 やること

JavaScript から**要素のクラスを付け外し**して、見た目を切り替えます。

## ✅ 要件

1. ボタン `#darkBtn` を押すたびに、`<body>` に `.dark` クラスを**トグル**（付け外し）する
2. ボタン `#addBtn` を押すと、`.box` に `.active` クラスを**追加**
3. ボタン `#removeBtn` を押すと、`.box` から `.active` クラスを**削除**
4. CSS で `.dark` と `.active` は定義済みなので、クラスを切り替えればスタイルが変わる

## 👀 確認方法

- 「ダークモード」ボタンで背景が黒⇔白に切り替わる
- 「追加」でボックスが赤色に、「削除」で元に戻る

## 💡 ヒント

| メソッド | 説明 |
| --- | --- |
| `element.classList.add('name')` | クラス追加 |
| `element.classList.remove('name')` | クラス削除 |
| `element.classList.toggle('name')` | あれば削除、なければ追加 |
| `element.classList.contains('name')` | 有無チェック |
