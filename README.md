# Studio Reservation System

## 作成背景
私が所属していた軽音楽部では、練習場所の予約を紙の掲示板で管理していました。これを改善し、いつでもどこからでも予約状況を確認できるように、このシステムを開発しました。  

## 使用した技術
PHP、HTML、CSS、およびMySQLを使用して開発しました。

## 使用方法
トップページでは利用日から1か月後までの予約状況を確認できます。  
予約状況を更新するためには、ログインが必要です。  
予約をする場合、ログインした状態で"予約する"ボタンをクリックし、バンド名を入力することで予約が完了します。  
予約の取り消しは、予約者のみ実行できます。トップページのバンド名をクリックし、予約の取消しページに移動することでキャンセルを行えます。  
  
アカウント作成時において、学籍番号欄は以下のフォーマットで入力する必要があります。  
　正規表現 "[e][1][a-z][0-9]{5}" 　 (例: "e1a11111" や "e1b12345" など）
 
## 著者
著者: 川崎海斗
