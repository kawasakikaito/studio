# Studio Reservation System

## 作成背景

私が所属していた軽音楽部では、練習場所の予約を掲示板の張り紙で管理していました。これを改善し、いつでもどこからでも予約状況を確認できるように、本システムを開発しました。

## 使用した技術

PHP、HTML、CSS、および MySQL を使用して開発しました。

## 使用方法

トップページでは利用日から 1 か月後までの予約状況を確認できます。<br>
予約または、削除をするためにはログインが必要です。<br>
予約をする場合、ログインした状態で"予約する"ボタンをクリックし、バンド名を入力することで予約が完了します。<br>
予約の削除は予約者のみが実行できます。トップページのバンド名をクリックし、予約の取消しページに移動することでキャンセルを行えます。<br>
<br>
アカウント作成時において、学籍番号欄は以下の正規表現に則って入力する必要があります。<br>
"[e][1][a-z][0-9]{5}" 　 (例: "e1a11111" や "e1b12345" など）

## 工夫した点

### トップページ(index.php)

- 文字数が 8 文字以上のバンド名は省略して表示

### ユーザー作成画面(signup.php)

- 学籍番号のフォーマットに正規表現を使用

- エラーを以下のパターン用意した
  1.  学籍番号が正規表現に則っていない場合
  2.  名前またはパスワードが空欄の場合
  3.  再確認用のパスワードと一致しない場合

### ユーザー確認画面(check.php)

- パスワードを hash 化してデータベースに登録

### 予約確認画面(register-check.php)

- 予約の重複を避けるように設計

## 著者

著者: 川崎海斗
