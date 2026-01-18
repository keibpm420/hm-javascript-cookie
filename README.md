## hm-javascript-cookie

Hello Mentor の課題で制作した、Cookie を使用した実装です。

### 概要

URL パラメータに含まれる `utm_source` を Cookie に保存し、
ページ読み込み時にその値を hidden フィールドへ自動でセットします。

### 仕様

-   URL に `utm_source` が存在する場合、Cookie に保存する
-   Cookie の有効期限は 30 日
-   Cookie に保存された値を `.js-utm-source` に自動入力する

### 使用例

以下のような URL でアクセスした場合、それぞれの値が Cookie に保存されます。

-   `https://example.com/?utm_source=map`
    → utm_source に `map` が保存される

-   `https://example.com/?utm_source=email`
    → utm_source に `email` が保存される

保存された値は、フォーム内の `.js-utm-source`（hidden フィールド）に自動でセットされます。

### 使用目的

流入元（広告・キャンペーン、メールなど）を判別するための実装です。
