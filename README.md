# app-memory-game

jQueryとBootstrapを使った対戦型トランプゲーム

## Feature

- ゲーム設定機能
  - ゲームに使用するトランプの柄・枚数・対戦相手の強さを設定する
  - 対戦中はゲーム設定に関する操作は無効となる
  - 「リセット」ボタンをクリックするとデフォルトの設定値に戻る
- チュートリアル機能
  - 「スタート」ボタンをクリックするとチュートリアルがモーダルに表示される
  - ゲームのルールと操作方法をカルーセル・ポップオーバ・CSSアニメーションで説明する
- 対戦機能
  - カードの裏面をクリックすると反転して表面の数字とマークが表示される
  - 対戦相手のターン中やすでに表になっているカードに対する操作は無効となる
  - 2枚のカードを選択して同じ数字が出た場合は現在のプレイヤがカードを獲得する
  - 2枚のカードを選択して違う数字が出た場合は次のプレイヤにターンが移る
  - ターンが次のプレイヤに移ったことをトーストで通知する
  - さきに全カード枚数の半数を獲得したプレイヤの勝利とする
- NPC機能
  - 対戦相手をプログラム制御（NPC）またはマニュアル制御（人間）から選択する
  - NPCは表になったカードの配置と数字を記憶する
  - NPCのターンになると記憶した情報を利用してカードを選択する
  - 同じ数字のペアを作れないときはランダムにカードを選択する
  - 記憶できる枚数の上限を超えた場合はランダムにカードを忘れる
  - 記憶してから時間が経っているカードほど忘れられやすい
  - 設定した強さにより記憶できる枚数の上限が決まる
- 進捗表示機能
  - 各プレイヤが獲得したカードの枚数とパーセントをプログレスバーに表示する
- 結果表示機能
  - どちらかが全カード枚数の50%以上を獲得した時点で結果をモーダルに表示する
  - 結果には勝利したプレイヤ名と獲得枚数と強さの設定を表示する

## Demo

### チュートリアル

![memory_game_tutorial](https://user-images.githubusercontent.com/49770211/79117945-74d06600-7dc7-11ea-9f4c-844b208c4af0.gif)

### 対戦中

![memory_game_play](https://user-images.githubusercontent.com/49770211/79117954-7bf77400-7dc7-11ea-9103-d6975390cc71.gif)

## Environments

- jQuery 3.4.1
- Bootstrap 4.4.1
- Illustrator
- Firebase Hosting

## Licence

This app is released under the [MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)
