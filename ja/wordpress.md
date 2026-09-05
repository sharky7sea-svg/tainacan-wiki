# WindowsのXAMPPサーバーにWordPressをインストールする方法 #

<br>

ローカルマシンへのWebサーバーのインストールに続いて、ここでは**WordPress**をインストールします。Webサーバーをまだインストールしていない場合は、[チュートリアルを見るにはこちらをクリック](/ja/xampp#ローカルのwindowsマシン（サーバーなし）にtainacanをインストールする)。
**Tainacan**をインストールするには、[こちらのチュートリアル](/ja/tainacan#wordpressにtainacanプラグインをインストールする方法)を参照してください。

同じチュートリアルを動画で見ることもできます。
* [XAMPP](https://www.youtube.com/watch?v=rznX0EZhWG4)
* [WordPress](https://www.youtube.com/watch?v=7v6qNHmqm0I)
* [Tainacan](https://www.youtube.com/watch?v=qRtoNRUlVkk)

## ダウンロード ##

まず、https://br.wordpress.org/download/ にアクセスし、**Windows**用の**WordPress**をダウンロードします。

![](/_assets/images/wordpress_01.png)

上の図で、ダウンロードするには**WordPress 5.2.1をダウンロード**をクリックします。処理が完了したら、ダウンロードしたファイルを解凍してインストールを開始します。

<br><br>

![](/_assets/images/wordpress_02.png)
**解凍**

圧縮ファイルを右クリックし、**すべて展開…**をクリックします。解凍が完了するまで待ちます。

<br><br>

![](/_assets/images/wordpress_03.png)

解凍したフォルダーを開き、**WordPress**フォルダーを右クリックして、**コピー**をクリックします。

<br><br>

![](/_assets/images/wordpress_04.png)

次に、`C:/xampp/htdocs`へ移動し、フォルダー内を右クリックして**貼り付け**をクリックします。

<br><br>

![](/_assets/images/wordpress_05.png)

上の画像は、転送処理が完了したフォルダーです。

<br><br>

![](/_assets/images/wordpress_06.png)

このプロジェクトでは、**WordPress**フォルダーの名前を**projeto_teste**に変更します。フォルダー名は自由に決めて構いませんが、作成するプロジェクト名を使用することをおすすめします。

<br><br>

## 新しいデータベースを作成 ##

![](/_assets/images/wordpress_07.png)

これで、**WordPress**の名前が変更され、正しい場所に配置されました。次に設定する必要があります。そのために、WordPressで使用するデータベースを作成します。ブラウザーで新しいタブを開き、`localhost/phpmyadmin`と入力します。

<br><br>

![](/_assets/images/wordpress_08.png)

これは**phpmyadmin**の画面です。ここでは、**XAMPP**に含まれるプロジェクトで使用されているデータベースを変更できます。ここで問題を起こさないよう十分注意してください。新しいデータベースを作成するには、左側の一覧にある**新規（New）**ボタンをクリックします。

<br><br>

![](/_assets/images/wordpress_09.png)

この画面で、**データベース名**フィールドにデータベース名を入力します。この例では**banco_teste**という名前を使用しますが、ここには好きな名前を入力できます。作成するプロジェクト名を使用することをおすすめします。入力が完了したら、**作成**ボタンをクリックします。

<br><br>

![](/_assets/images/wordpress_10.png)

この画面は、データベースが作成され、空であることを示しています。左側の一覧にある名前に注目してください。

<br><br>

## データベースをプロジェクトに接続 ##

![](/_assets/images/wordpress_11.png)

次に、`localhost/projeto_teste`というアドレスで新しいタブを開きます。
このサイトを開くのは初めてなので、最後の設定が実行されます。

<br><br>

![](/_assets/images/wordpress_12.png)

データベースを作成したので、インストールを続行するには**始めましょう！**をクリックします。

<br><br>

![](/_assets/images/wordpress_13.png)

この画面では、次の情報を入力する必要があります：
1. 作成した**データベース**の名前。
2. データベースへのアクセスに使用する**ユーザー名**。**XAMPP**では通常、ユーザー名に**root**を使用します。
3. データベースへのアクセスに使用する**パスワード**。**XAMPP**では通常、パスワードを空欄にします。
4. **データベースサーバー**と**テーブル接頭辞**は変更する必要がありません。

<br><br>

![](/_assets/images/wordpress_14.png)

この例では、データは上の画像のようになります。最後に、ページ下部にある**送信**ボタンをクリックします。

<br><br>

![](/_assets/images/wordpress_15.png)

この画面は、インストールのこの部分が完了したことを示しています。上の画像のように、**インストール**ボタンをクリックします。

<br><br>

## 最後の設定 ##

![](/_assets/images/wordpress_16.png)

すべて順調なら、この画面が表示されます。ここでは、**管理画面**（**admin**）へのアクセスに使用する**サイトのタイトル**、**ユーザー名**、**パスワード**、サイト管理者の**メールアドレス**、**google**などのサイトにおける**表示設定**などを設定します。すべてのフィールドに適切な内容を入力し、ページ下部にある**WordPressをインストール**をクリックします。

<br><br>

![](/_assets/images/wordpress_17.png)

これで準備完了です。**WordPress**がインストールされました。サイトを表示するには**ログイン**をクリックします。

<br><br>

## 管理画面 ##

![](/_assets/images/wordpress_18.png)

上の画像のように、**管理画面**のログイン画面が表示されます。選択した**ユーザー名**と**パスワード**を入力してアクセスします。

<br><br>

![](/_assets/images/wordpress_19.png)

これは**WordPress**の**管理画面**です。サイト上のすべてのものを、この画面のオプションで変更できます。サイトを表示するには、上部左側にある選択したタイトルを、上の画像で示されているようにクリックします。

<br><br>

![](/_assets/images/wordpress_20.png)
**WordPressのホーム**

これで完了です。次回以降、サイトに直接アクセスする場合は、`localhost/projeto_teste`（または選択した名前）にアクセスするだけです。
**管理画面**に直接アクセスするには、`localhost/projeto_teste/wp-admin`（**projeto_teste**の代わりに選択した名前）にアクセスします。

これで、[Tainacan](/ja/tainacan#wordpressにtainacanプラグインをインストールする方法)プラグインのインストールを開始できます。

<br><br>
