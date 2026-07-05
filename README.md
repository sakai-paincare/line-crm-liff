# line-crm-liff

LINE公式アカウント「デジタル診察券」LIFFページ(GitHub Pages配信用)。

このリポジトリは **GitHub Pagesで公開するための静的ページ1枚だけ** を置く。
本体(GAS・運用ドキュメント)は private リポジトリ `line-crm` にある。
セットアップ手順は line-crm の `docs/liff-card.md` 参照。

- ルート直下 … テスト環境(テスト用チャネル)向け
  - `index.html` … デジタル診察券ページ。冒頭の `LIFF_ID` / `API_URL` を直接編集する
  - `track.html` … リッチメニュータップ計測リダイレクトページ(美容枠で稼働中)
  - `reserve.html` … 予約導線の2択ページ(WEB予約 / LINEで予約希望)
- `nagasaki/` … ながさきハートクリニック本番向け(card / track / reserve の3ページ。
  冒頭の `LIFF_ID` / `API_URL` は長崎のLoginチャネル・GAS作成後に記入)
- `fukuoka/` … 福岡本番向け(本番移行時に作成。line-crm の docs/production-migration.md 参照)
- 公開URL: https://sakai-paincare.github.io/line-crm-liff/ (各ページは `/<ディレクトリ>/<ファイル名>` )
- LIFFエンドポイントURLに上記を設定する

**患者データ・トークン類は絶対にこのリポジトリに置かないこと**(publicリポジトリのため)。
