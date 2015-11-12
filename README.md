# [general_form](https://github.com/taromorimotohf/general_form/)

## NOT GENERAL FORM
### 基本的なフォームの機能を実装（添付画像あり）
・ [PHPMailer](https://github.com/PHPMailer/PHPMailer)を使用。
・他は基本的な機能のみ（現在、タイトル、、メールアドレス、メッセージ、添付画像1枚のみ）

## Get Started
###1.send.phpが設定ファイルも流用している。
```rb
    /**
    * 設定ファイル
    */
    $remail = 1; // 1 送る。　0 送らない。
    $mailto = $_SESSION['mail'];//自動返信先
    $mailto02 = 'taro_morimoto@hot-factory.jp';//管理者メールアドレス
    $subject  = "お問い合わせがありました"; //自動返信タイトル
    $subject02  = "【管理者】お問い合わせ"; //管理者自動返信タイトル  
    $mailfrom = "sender@test.com";   
    $fromname = "◎◎株式会社";  
```

###2.添付画像を一時的にアップロードフォルダはパーミッション「777」にしてください。
###2.send.phpのコメントを読んで使えない場合は使用は申し訳ありませんが、控えてください。

## WHAT'S NOT GENERAL?
・まだまだ足りないフォームです。なので、、、
・上記項目以外の追加に関しては自己責任でお願いします。なので、、すいません。

## SOURCE CHECK PLEASE!!
どなたか是非お願いします。

現状
----------------------
・リファラーチェック
・ワンタイムチケット
・htmlspecialchars
----------------------

のみ対応しています。
## FEATURE THIS UPDATE
・ラジオボタン、プルダウン、セレクトボックス追加予定
・添付画像を最大5個まで使用可能にしたい。（アップロード最大サイズも変数で持たせるように。）
・configファイルを作成予定。
・[angular.js](https://angularjs.org/)を使ってリアルタイムバリデート予定。

#という感じです。すいません。　2015.11.12 TARO

#### Directory
```
 input.php ..................... フォームの入力画面
 confirm.php ..................... フォームの確認画面
 send.php ..................... フォームの送信画面及び、設定ファイル
 class.phpmailer.php ..................... メール送信クラス（外部SMTPを使わなければこれだけでいいかと。。。）
 class.phpmaileroauth.php ..................... 必要ないかも（というかよくわかってない）。。
 class.phpmaileroauthgoogle.php ..................... 必要ないかも（というかよくわかってない）。。
 class.pop3.php ..................... 必要ないかも（というかよくわかってない）。。
 class.smtp.php ..................... 外部SMTPを利用する場合。
 files ..................... 一時画像フォルダ
```
