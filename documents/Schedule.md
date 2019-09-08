# ゲーム開発スケジュール

## コンセプトを決める

[x] ゲームのコンセプトを考える
[x] ゲームのゴールを考える

## 仕様を決める

[x] ゲームの仕様を決めるスケジュールを考える
[x] 9/7 ゲーム全体の流れ、画面要素を洗い出す
[ ] 9/8 ゲームに必要なデータを洗い出す
[ ] 9/14 ゲームのアーキテクチャを考える

## 開発の準備スケジュールを決める

[x] ゲームの開発の準備のスケジュールを考える
[ ] (10day) 基本技術の習得(最優先)
    [ ] (5day) APP:  React/Redux → TODOアプリ on Docker
    [ ] (2day) UI:   Semantic-ui-react
    [ ] (2day) TEST: mocha,
[ ] (3day) 開発環境を整える
    [ ] Docker
    [ ] MySQL
    [ ] Laravel
    [ ] Webpack
    [ ] node - npm - yarn
        [ ] eslint
        [ ] prettier
        [ ] semantic-ui-react
    [ ] React
    [ ] TypeScript
    [ ] TestSystem
    [ ] BuildSystem

## 本開発のスケジュールを決める

[ ] 必要な機能を考える
    [ ] (1day) どんな機能が必要か洗い出す
    [ ] (2day) どれくらいの工数がかかるのかざっくり見積もる
        - 24時間を1スプリントとしてざっくり工数をだす。あぶれるなら分解する。
    [ ] (1day) どういう順番で作っていくか考える
    [x] どのタイミングでスケジュールを見直すか決めておく
        - ２週間ごとくらい

## 開発を始める

- 優先度の高いものから順番に実装する
- 出来るだけ体系的に開発する
    - End to End な作業に終始する
    - 動いたらリファクタリングする
    - Test も 実装する
    - 常に動く状態を維持してコミットする

## 個別の開発を行うフロー

[ ] 調査：機能の仕様を細かいところまで洗い出す
    [ ] 何が必要で(Input), どういう結果になる機能なのか(Output) を明確にする
    [ ] テストを作成する
[ ] 見積：機能の工数を算出する 
[ ] 実装：一つ一つ開発を進める。featureブランチにコミットする
[ ] テスト：テストを回して、動作をチェックする
[ ] 整理：リファクタリングを考える
[ ] テスト：再度テストを回して、動作をチェックする
[ ] 納品：開発したものをコミットし、PRを出し、マージする

# 基本技術を習得する

[ ] (10day) 基本技術の習得(最優先)
    [ ] (5day) APP:  React/Redux → TODOアプリ on Docker
    [ ] (2day) UI:   Semantic-ui-react
    [ ] (2day) TEST: mocha,

## 参考文献

- Redux Saga https://redux-saga.js.org/
- Redux の流れについて細かいステップで解説してくれた https://www.codingame.com/playgrounds/9169/simple-redux-create-delete-contact-application