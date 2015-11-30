# 20151125-sample-6
# Cloud9とは
 Cloud9（クラウド9）とはアプリケーションの開発やデータベースなどをクラウド環境で利用できるサービスです。
### Cloud9の登録方法
GitHubのアカウントをお持ちの場合は、GitHubのアカウントでログインすることも可能です。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/e01597d772928215d56a82164343d2cc-620x188.png" >
###ワークスペースの作成方法
登録が完了するとダッシュボード画面が表示されるので、「Create a new workspace」ボタンを押してください。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/fb9b1556d81026464d57cb004f2db222-620x348.png" >
###基本的な使い方
ファイルを作成するには、左のフォルダが表示されている箇所で右クリックをして「New File」を選択すると作成できます。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/cloud9_021-620x348.png" >
<br>フォルダを作成する際も同じ要領で右クリックしてから「New Folder」を選択すると作成できます。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/cloud9_032-620x348.png" >
###Apacheを起動してプレビューする
Cloud9では、Apacheを起動して開発している内容をプレビューすることができます。
ファイルを作成して「Run」のボタンをクリックすると、画面の下部にこのようなリンクが表示されるのでクリックしてください。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/cloud9_09-620x348.png" >
<br>すると、プレビューがCloud9上に表示されました。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/cloud9_10-620x348.png" >
<br>このプレビューはURLをコピーして自分が使っているブラウザで表示するもできます。
###ワークスペースを共有する
<br>Cloud9では、自分で開発しているワークスペースを他の人に共有することが可能です。 ただし、共有するにはちょっとした設定が必要になります。
ワークスペースの右上に「Share」のボタンをクリックするとこのような画面が表示されます。ここでPublicのチェックを外さないようにしましょう。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/cloud9_06-620x349.png" >
<br>エディタを共有するには、Editorに表示されているURL共有します。URLをクリックして、表示された「Copy」をクリックするとコピー可能です。このコピーしたURLを共有したい人に開いてもらいましょう。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/cloud9_07-620x348.png" >
<br>URLに他の人がアクセスすると「Notifications」に表示されますので、緑のボタンをクリックして許可するとそのユーザーが編集まで可能になります。ペアプログラミングなどもできるので便利です。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/cloud9_08-620x348.png" >
<br>また、毎回許可するのではなく、特定のユーザーに閲覧・編集の権限を付与することも可能です。
<br>先ほどのShareボタンを押した時に表示される画面の下部に「InvitePeople」というフォームがあるので、共有したい人のユーザー名を入れて「Invite」ボタンを押してください。

<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/cloud9_invite.png" >
<br>
このように表示されれば成功です。
<br>
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/cloud9_invite_completed.png" >

###テンプレートを使ってみる
<br>ここまでは「Custom」を使って紹介してきましたが、Cloud9には便利なテンプレートが用意されています。今回は、Ruby on <br>RailsとWordPressのテンプレートを実際に使ってみます。
####Ruby on Railsのテンプレート
<br>テンプレートの1つ目として、Ruby on Railsのテンプレートを使用します。
<br>まずはテンプレートで「Ruby」を選びましょう。
<br><img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/ruby1-620x216.png" >
<br>選択して開くだけでRuby on Railsの開発環境が構築できた状態になります。
<br><img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/Rails-620x315.png" >
<br>Railsアプリケーションを起動する場合は、通常「railss」コマンドを使用しますが、Cloud9では下記のコマンドを入力します。コンソール部分でこのように入力してください。

$ rails s -p $PORT -b $IP

<br><img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/console_png-620x544.png" >
<br>コマンド入力後、このように表示されればサーバは正常に起動しています。
<br>=> Booting WEBrick
=> Rails 4.1.6 application starting in development on http://0.0.0.0:8080
=> Run `rails server -h` for more startup options
=> Notice: server is listening on all interfaces (0.0.0.0). Consider using 127.0.0.1 (–binding option)
=> Ctrl-C to shutdown server
[2015-06-08 05:10:45] INFO WEBrick 1.3.1
[2015-06-08 05:10:45] INFO ruby 2.1.5 (2014-11-13) [x86_64-linux]
[2015-06-08 05:10:45] INFO WEBrick::HTTPServer#start: pid=2367 port=8080

<br>起動するとこのようにURLが表示されるので、クリックしてアクセスしてください。
<br><img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/rails-s-620x193.png" >
<br>アクセスするとアプリケーションの初期画面が表示されます。
<br>この初期画面ではRubyのバージョン、実行しているアプリケーションの情報などが閲覧できます。
<img src="http://static.techacademy.jp/magazine/wp-content/uploads/2015/07/rails-top-620x455.png" >
<br>なお、コンソール上でCtrl + cを押すと、railsのwebサーバが停止します。
<br>以上が、Ruby on Railsのテンプレートの使い方です。
