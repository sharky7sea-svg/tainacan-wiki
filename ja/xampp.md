# ローカルのWindowsマシン（サーバーなし）にTainacanをインストールする #

<br>

**Tainacan**は**WordPress**の**プラグイン**です。何もインストールされていない場合、使用するには次の3つの簡単なインストールを行う必要があります。
1. マシン上のWebサーバー。ここでは[WindowsにXAMPPをインストールする方法](#ダウンロード)を説明します。
2. **WordPress**。[XAMPPサーバー（Windows）にWordPressをインストールする方法](/ja/wordpress#windowsのxamppサーバーにwordpressをインストールする方法)を参照してください。
3. **Tainacan**プラグイン。[WordPressにTainacanをインストールする方法](/ja/tainacan#wordpressにtainacanプラグインをインストールする方法)を説明しています。

## ダウンロード ##

まず、https://www.apachefriends.org/en/index.html にアクセスし、**Windows**用の**XAMPP**をダウンロードします。

![](/_assets/images/xampp_01.png)

上の画像で、**XAMPP for Windows 7.3.6 (PHP 7.3.6)**ボタンをクリックしてダウンロードを開始します。処理が終わったら、ダウンロードしたファイルを実行してインストールを開始します。

<br><br>

## インストール ##

![](/_assets/images/xampp_02.png)

これは初期インストール画面です。「次へ」(Next)ボタンをクリックします。

<br><br>

![](/_assets/images/xampp_03.png)

これはインストールするコンポーネントを選択する画面です。何も変更する必要はありません。もう一度「次へ」(Next)をクリックします。

<br><br>

![](/_assets/images/xampp_04.png)

この画面では、プログラムのインストール場所を尋ねられます。ここでも変更する必要はありません。「次へ」(Next)をクリックします。

<br><br>

![](/_assets/images/xampp_05.png)

この画面には、インストーラーライブラリであるBitnamiが表示されます。ここでも変更する必要はありません。「次へ」(Next)をクリックします。

<br><br>

![](/_assets/images/xampp_06.png)

ここでは警告メッセージだけが表示されます。インストールを開始する準備ができました。「次へ」(Next)をクリックして処理を開始します。

<br><br>

![](/_assets/images/xampp_07.png)

インストールが実行されています。バーが完全に埋まるまで待ちます。

<br><br>

## コントロールパネルを開く ##

![](/_assets/images/xampp_08.png)

処理が完了し、インストールが終わりました。チェックボックスを選択したまま「完了」(Finish)をクリックします。これにより現在の画面が閉じ、その後すぐにコントロールパネルの画面が表示されます。

<br><br>

![](/_assets/images/xampp_09.png)

言語選択ボックスが表示されます。最初の選択肢である英語 (English)を選びます。その後、「保存」(Save)をクリックします。

<br><br>

![](/_assets/images/xampp_10.png)

上の画像のようにコントロールパネルが表示されます。**XAMPP**を動作させるには、**Apache**と**MySQL**のサービスにある「開始」(Start)ボタンをクリックする必要があります。
注：サーバーを使用するときは、必ずこの2つのサービスを有効にする必要があります。

<br><br>

![](/_assets/images/xampp_11.png)

すべてが正常に進めば、上の画像のように両方のサービスが緑色になります。次に「管理」(Admin)ボタンをクリックします。使用しているメインブラウザー（**Google Chrome**、**Firefox**、**Internet Explorer**など）が開き、`localhost/dashboard`のアドレスがすでに入力された状態になります。

<br><br>

## テスト ##

![](/_assets/images/xampp_12.png)

インストールが問題なく完了していれば、上の画面が表示されます。これでサーバーは正常に動作しています。次に、ブラウザーに表示するファイルを保存するフォルダーに移動します。

<br><br>

![](/_assets/images/xampp_13.png)

上の画像で、フォルダーのアドレス`C:/xampp/htdocs`を確認できます。
ブラウザーで表示するファイルはここに保存します。
これで、**Windows**上で**XAMPP**サーバーが動作するようになりました。

<br><br>

次は、**XAMPP**サーバーに[WordPress](/ja/wordpress#windowsのxamppサーバーにwordpressをインストールする方法)をインストールします。

<br><br>
