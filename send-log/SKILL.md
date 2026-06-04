---
name: send-log
description: ログ送信の処理を実装するスキル
---

# Send Log

## Instructions

1. ログ送信対象のエレメントをユーザーに確認する
2. 対象エレメントの `js-` プレフィックスクラスの有無を確認する
   - **ある場合**: イベントリスナー内で `sendLog()` を呼び出す
   - **ない場合**: `js-` プレフィックスクラスを HTML 要素に追加してから、イベントリスナー内で `sendLog()` を呼び出す
3. [GUIDLINE.md](./GUIDLINE.md) のルールを遵守する

## Example

### `js-` クラスがある場合

```html
<button class="button js-button">ボタン</button>
```

`js-button` のイベントリスナー内で `sendLog()` を呼び出す。

### `js-` クラスがない場合

**変更前:**
```html
<button class="button">ボタン</button>
```

**変更後:**
```html
<button class="button js-button">ボタン</button>
```

`js-button` クラスを追加し、イベントリスナー内で `sendLog()` を呼び出す。
