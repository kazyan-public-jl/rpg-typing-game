# ゲームの全体構成要素

ゲームの開発に必要となる次の項目について考えをまとめる

- アーキテクチャ（インフラ環境）
- 画面仕様
- マスターデータ設計


# アーキテクチャ

- ざっくりとどんな構成で作ろうか考える。
- 使ったことのある技術の練度を高めるのも目的の一つなので、以下のような構成になりそう。
- どこからどこまでを何で担保するか、明確にしておかないと、ぐちゃぐちゃになりそう。慎重に。
- 随時追加していく。

## フロントエンド

基本的にここだけで動くような作りから始めたい。

その先に Laravel-MySQL あたりを連携する方が楽ならばそれも導入していきたい

- 基本技術: HTML5
- 動作制御: Javascript ES6/React
- データ管理: Redux 

## サーバーサイド

- ネットワーク的な処理をしたい場合に利用する
- DBとのやりとりを行う
- ブラウザに置いておきたくない静的ファイルを取得する関数など

- PHP
- Laravel

## リソース

マスターデータやよく使う画像など

- csv
    - 各種マスターデータ
- image
    - background-image
    - icon
    - ui-parts

## データベース

永続化したいデータ、リロードしても消えないデータをここに退避しておく

LocalStorageを使いすぎない方がいいかもしれない

- LocalStorage
    - Pros: ブラウザだけでKVSができる。5MBまで可能。
    - Cons: テキストしか保存できない。JSONは文字列変換が必要。ブラウザ間のデータ共有ができない。
- MySQL
    - Pros: 世界一のDBサービス。
    - Cons: サーバーが必要となる。
- AWS サービス
    - Pros: 既定のサービスが豊富。うまく使えれば環境構築が圧倒的に楽。
    - Cons: 使えるようになるまでの学習コストが高そう。

## 画像

自作は厳しいので、出来るだけフリー素材で作りたい

- フリー素材
    - イラストや: https://www.irasutoya.com/
    - フリーアイコン: https://sozai.cman.jp/icon/tile/square/
- フリーアイコンライブラリ
    - Font Awesome: https://fontawesome.com/icons?d=gallery&m=free
        - 使い方の例: https://saruwakakun.com/html-css/basic/font-awesome
    - Semantic UI React - Icon: https://react.semantic-ui.com/elements/icon/

