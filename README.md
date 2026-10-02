# salon-pages

各サロンの、インスタのプロフィールに貼る予約の入口ページです。GitHub Pagesで公開しています。

| お店 | ページ |
| --- | --- |
| sample-salon | https://kamiya777.github.io/salon-pages/sample-salon/ |

お店ごとのフォルダには2つのページがあります。

- `index.html`：インスタのプロフィールに貼る入口ページ
- `reserve/index.html`：予約画面。`salon-booking-gas-core/src/index.html` のコピーで、`<meta name="booking-api">` にそのお店のGASのウェブアプリのURL（/exec）を入れてあります

お店を追加するときは、フォルダをコピーして名前を変え、次を書き換えます。

1. `index.html` の上のほうにある「お店ごとに書き換えるところ」
2. `reserve/index.html` の `booking-api` の URL
3. そのお店のスプレッドシートの「設定」シートの「予約ページURL」に、`https://kamiya777.github.io/salon-pages/<フォルダ名>/reserve/` を入れる（メールのキャンセル用リンクに使います）

予約画面（`salon-booking-gas-core/src/index.html`）を直したときは、各お店の `reserve/index.html` にもコピーし直します。
