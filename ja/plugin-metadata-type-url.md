# プラグイン：Tainacan URL Metadata Type

このプラグインは、追加のメタデータタイプに対応することでTainacanプラグインの機能を拡張します。これは、_WordPress_の自動埋め込み機能を使うか、iframeの使用を強制して、URLリンクを埋め込みコンテンツとして表示するのに役立ちます。URLタイプのドキュメントを複数持ちたい場合や、添付ファイル一覧でもURLを受け付けたい場合に適したソリューションです。

## インストール

_WordPress_のプラグインページで「Tainacan」を検索し、「Tainacan URL Metadata Typeプラグイン」を有効化します。[このリンク](https://github.com/tainacan/tainacan-metadata-type-url ":ignore")からも確認できます。そこからボタンを押してインストールできます。

お好みで、[.zip](https://github.com/tainacan/tainacan-metadata-type-url/releases ":ignore")ファイルを[GitHubリポジトリ](https://github.com/tainacan/tainacan-metadata-type-url ":ignore")からダウンロードし、[プラグインのインストール手順](/ja/plugins#プラグインのインストール)に記載されたインストール手順に従うこともできます。

WordPress管理画面のプラグインセクションで、このプラグインを有効化します。

## 使用方法

コレクションまたはリポジトリのメタデータページに移動します。「利用可能なメタデータタイプ」一覧に、URLタイプが表示されているはずです。それを選択し、好きな名前を付けて新しいメタデータを作成します。デフォルトでは、このプラグインは_WordPress_の自動埋め込み方式を使用して、リンクのプレビューを表示しようとします。この方式で機能するリンクには、YouTube、Twitter、Spotifyなどの[限られた一覧](https://wordpress.org/support/article/embeds/#okay-so-what-sites-can-i-embed-from ":ignore")があります。リンクがその一覧にない場合（たとえばGoogle Mapsのリンク）でも、アイテムのメタデータ一覧にコンテンツのプレビューを表示したいときは、「iframeを強制（Force iframe）」オプションと関連設定を指定できます。

![メタデータ設定画面のスクリーンショット](/_assets/images/plugins_metadata_type_url_screenshot-1.png)

> [!NOTE]
> 「iframeを強制（Force iframe）」を使用しても、リンク先のURLによってはiframeでの埋め込みが許可されず、リンクを表示できない場合があります。これはサイト作成者が有効にしている設定であり、無視することはできません。

メタデータの準備ができたら、新しいアイテムを作成し、そこにURLの値を入力します。アイテム編集フォームでプレビュー表示ボタンをクリックするか、アイテムページにアクセスして表示された内容を確認できます。

<div style="display: flex;flex-wrap: wrap; justify-content: space-around;">

![YouTube動画を含むアイテム作成フォームのスクリーンショット](/_assets/images/plugins_metadata_type_url_screenshot-2.png ":size=380")

![Google Mapsリンクを含むアイテム作成フォームのスクリーンショット](/_assets/images/plugins_metadata_type_url_screenshot-3.png ":size=380")

</div>

![埋め込みリンクを含むアイテムページのスクリーンショット](/_assets/images/plugins_metadata_type_url_screenshot-4.png)
