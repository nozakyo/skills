# skills

GitHub Copilot のカスタムスキル一覧。

## スキル一覧

### [code-review](./code-review/)

コードのレビュー・修正を行うスキル。

[GUIDLINE.md](./code-review/GUIDLINE.md) に定義されたレビュー観点（命名規則・HTML/CSS/JS の品質・コメントルールなど）に従ってコードをチェックする。

### [send-log](./send-log/)

ログ送信の処理を実装するスキル。

対象要素の `js-` プレフィックスクラスの有無を確認し、[GUIDLINE.md](./send-log/GUIDLINE.md) のルールに従って `sendLog()` を呼び出すイベントリスナーを追加する。
