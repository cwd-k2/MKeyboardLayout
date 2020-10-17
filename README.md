# MKeyboardLayout

日本語ローマ字入力（及び英語入力）に特化したキーボードレイアウト

## 配列

![layout](https://github.com/cwd-k2/MKeyboardLayout/blob/master/resources/keylayout.png)

ここに示してあるのは配列の一部のみです．
それ以外の，記号等の配列については特に指定していません．

## 特徴

- 母音、子音が左右に分かれていることで交互打鍵の割合を多くした
- 母音・子音それぞれの配置も，日本語入力時の登場頻度を基に設計
  - 暗黙の前提として，人差し指・中指＞薬指＞小指の順に指の強さがあると仮定しています
- 英語は二の次

## 利用してみる

### macOS

1. [Dropbox のリンク](https://www.dropbox.com/s/nwg4kytxxgvsdgo/M%2B%2B.keylayout?dl=0)から `M++.keylayout` をダウンロードします．
1. `~/Library/Keyboard Layouts` に `M++.keylayout` をコピーまたは移動します．これでインストールが完了します．
1. (必須かどうかはわかりませんが) ログインしなおす，または OS を再起動します．
1. `システム環境設定 > キーボード > 入力ソース` から入力ソースとして `M++` を追加します (その他に分類されています)．
![01](https://github.com/cwd-k2/MKeyboardLayout/blob/master/resources/01.png)
![02](https://github.com/cwd-k2/MKeyboardLayout/blob/master/resources/02.png)
1. 日本語入力のキー配列として利用したい場合，日本語入力の「英字のレイアウト」のドロップダウンから `M++` を選択することで実現可能です．
![03](https://github.com/cwd-k2/MKeyboardLayout/blob/master/resources/03.png)
![04](https://github.com/cwd-k2/MKeyboardLayout/blob/master/resources/04.png)

このリンクに用意してある `M++.keylayout` は [Ukelele](https://software.sil.org/ukelele/) というソフトウェアで作成したものです．JIS 配列用のものしか作っていませんので，その他の US 配列などのキーボードではどうなるか分かりません．

## やること

- 各環境用にキー配列を実現するファイルを用意する

## やりたいこと

- 簡単な形式のキー配列の定義から自動的に各種環境用のファイルを生成する仕組み
- キー配列の評価・可視化をするプログラム
