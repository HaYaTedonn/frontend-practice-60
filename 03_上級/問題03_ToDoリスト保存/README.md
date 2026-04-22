# 上級 問題03: ToDoリスト（保存機能付き）

**難易度: ★★★★★★☆☆☆☆**

## 🎯 やること

中級 問題19 の ToDo リストを、**LocalStorage に保存**してリロード後も復元するようにします。

## ✅ 要件

1. タスクは**配列**として管理し、JSON で LocalStorage に保存
2. 各タスクは `{ id, text, done }` の形
3. 追加・削除・チェック状態変更のたびに保存
4. 起動時に LocalStorage から復元
5. **再描画関数** `render()` を使い、配列が変わるたびに UI 全体を再構築
6. 完了済みタスクは `.done`、テキストに取り消し線

## 💡 ヒント

```js
let todos = JSON.parse(localStorage.getItem('todos')) || [];
function save() { localStorage.setItem('todos', JSON.stringify(todos)); }
function render() { /* todos を元に UL を作り直す */ }
```

`id` には `Date.now()` や `crypto.randomUUID()` を使う。
