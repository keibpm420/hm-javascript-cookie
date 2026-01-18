## Cookie（utm_source の管理）

Hello Mentor の課題で制作した、Cookie を使用した実装です。

### 概要

URL パラメータに含まれる `utm_source` を Cookie に保存し、
フォーム送信時にその値を自動で hidden フィールドへセットします。

### 仕様

-   URL に `utm_source` が存在する場合、Cookie に保存する
-   Cookie の有効期限は 30 日
-   Cookie に保存された値を `.js-utm-source` に自動入力する

### 使用目的

流入元（広告・キャンペーンなど）を判別するための実装です。
