# line-crm-liff

LINE公式アカウント「デジタル診察券」LIFFページ(GitHub Pages配信用)。

このリポジトリは **GitHub Pagesで公開するための静的ページ1枚だけ** を置く。
本体(GAS・運用ドキュメント)は private リポジトリ `line-crm` にある。
セットアップ手順は line-crm の `docs/liff-card.md` 参照。

- `index.html` … LIFFページ本体。冒頭の `LIFF_ID` / `API_URL` を直接編集する
- 公開URL: https://sakai-paincare.github.io/line-crm-liff/
- LIFFエンドポイントURLに上記を設定する

**患者データ・トークン類は絶対にこのリポジトリに置かないこと**(publicリポジトリのため)。
