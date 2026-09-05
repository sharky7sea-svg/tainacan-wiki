# プラグイン：追加表示モード

このプラグインは、コレクション設定で利用できる表示モードの一覧に、8つの追加表示モードオプションを追加します。

## はじめに

デフォルトでは、すべてのTainacanコレクションで、アイテム一覧を次の7つの表示モードで表示できます：

- Table（テーブル）
- Cards（カード）
- Records（レコード）
- Masonry（メーソンリー）
- Thumbnails（サムネイル）（Tainacanテーマを使用する場合）
- List（リスト）
- Slideshow（スライドショー）

これらのほとんどは管理画面の一覧表示でも利用できます。このプラグインは、インストールしたテーマ側（Webサイト自体）に表示される追加の表示モードをインストールします。これらはTainacanのデフォルトのデザインガイドラインには従いません。Tainacan開発の初期に、このようなカスタマイズが可能であることを示すために作成されました。また、[独自の表示モードを作成する方法](/dev/extra-view-modes)を学びたい開発者にとって、よい最初の一歩になります。公式ページの[この投稿](https://tainacan.org/blog/2018/06/13/custom-view-modes-how-will-the-world-see-your-collection/)でも、新しい表示モードを使用する可能性について説明しています。

利用できる新しい表示モードは次のとおりです：

1. **Gallery（ギャラリー）** - 2つのメタデータを表示し、スライダー付きライトボックスを開く、メーソンリー形式の表示モードです。
2. **Mosaic（モザイク）** - アイテムのサムネイルを余白なしで並べる、シンプルなモザイクです。
3. **Frame（フレーム）** - ギャラリー展示のように、中央揃えのフレーム付きサムネイルを表示します。
4. **Exhibition（展示）** - 画像とメタデータがマウスオーバー時に展開される、フレーム付きのレコード表示です。
5. **Albums（アルバム）** - ディスクを内側に配置したアルバムカバーのように、サムネイルを表示します。
6. **Document（ドキュメント）** - 公開された研究を表示するための、紙を重ねたスタイルのレコードです。
7. **Books（書籍）** - 図書館での表示に適した、本の表紙形式の表示です。
8. **Polaroid（ポラロイド）** - ポラロイド写真に似た、フレーム付きの写真表示です。

## インストール

_WordPress_のプラグインページで「Tainacan」を検索し、「Tainacan Extra View Modesプラグイン」を有効化します。[このリンク](https://wordpress.org/plugins/tainacan-extra-view-modes/ ":ignore")からも確認できます。そこからボタンを押してインストールできます。

お好みで、[.zip](https://github.com/tainacan/tainacan-extra-viewmodes/releases ":ignore")ファイルを[GitHubリポジトリ](https://github.com/tainacan/tainacan-extra-viewmodes ":ignore")からダウンロードし、[プラグインのインストール手順](/ja/plugins#プラグインのインストール)に記載されたインストール手順に従うこともできます。

WordPress管理画面のプラグインセクションで、このプラグインを有効化します。

## 設定

コレクションの設定ページに移動します。「利用可能な表示モード」セクションを探し、テーマの一覧で使用したいものにチェックを入れます：

![希望する表示モードの設定](/_assets/images/plugins_extra_view_modes_1.png ":size=420")

## 使用方法

これで完了です。異なるスタイルで一覧を表示できるようになりました。以下は、利用可能な表示モードで撮影したスクリーンショットです：

<div style="display: flex;flex-wrap: wrap; justify-content: space-around;">

![Gallery（ギャラリー）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-1.png ":size=320")

![ライトボックスを開いたGallery（ギャラリー）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-2.png ":size=320")

![ライトボックスとメタデータを開いたGallery（ギャラリー）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-3.png ":size=320")

![Mosaic（モザイク）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-4.png ":size=320")

![Frame（フレーム）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-5.png ":size=320")

![Exhibition（展示）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-6.png ":size=320")

![Albums（アルバム）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-7.png ":size=320")

![Document（ドキュメント）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-8.png ":size=320")

![Books（書籍）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-9.png ":size=320")

![Polaroid（ポラロイド）表示モードのスクリーンショット](/_assets/images/plugin_extra_viewmodes_screenshot-10.png ":size=320")

</div>
