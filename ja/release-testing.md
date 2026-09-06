> [!NOTE]
> このページの原文は*ブラジルポルトガル語*で提供されています。

# テスト手順

このセクションでは、Tainacan WordPressプラグインのインストールまたは更新時に完全性テストを行うための手順を説明します：

## リリース候補（Release Candidate / RC）のリリースフロー

これは、Tainacanプラグインの新しいバージョンがコミュニティによって事前に検証され、バグがある状態でWordPressリポジトリに送られることを防ぐための手順です：

1. [Tainacanコミュニティ](https://tainacan.discourse.group)でRC版を告知し、使用テストを実施してもらう；
2. 次の[テスト手順](#プラグインのテスト手順)に従ってテストを行う；
3. 見つかった問題を解決し、テストで問題が指摘されなくなるまで新しいRC版（Release Candidate）をリリースする。
4. その後、WordPress向けの[新しいバージョンをリリースする](/dev/release.md)手順に従う。

## プラグインのテスト手順

この手順は、Tainacanプラグインの機能が適切に動作し、プロセスを実行できることを確認するテストを行うためのものです。

> [!NOTE]
> 見つかった問題は[TainacanのGitHubのissue](https://github.com/tainacan/tainacan/issues ":ignore")またはTainacanの[コミュニティフォーラム](https://tainacan.discourse.group ":ignore")に報告できます。ページが読み込まれないなどの一般的なエラーは、[FAQページの提案](/ja/faq#エラーを見つけたと思います。どうすればよいですか？)を使用すると、より詳しく説明できます。

可能な限り多くの機能を対象にするため、実施できるテストにはさまざまな種類があります。すべて次の基本手順から始めます：

![Tainacanの管理メニュー](/_assets/images/release-testing-1.png ':class=alignright')

1. Tainacanプラグインのテストバージョンがインストールされ、有効化されている**WordPressの管理画面**にアクセスする（通常は、サイトのアドレスに`/wp-admin`を加えたもの）；
2. 左側のサイドバーで、Tainacanセクションの**インストール診断**をクリックする：
3. _Tainacanプラグイン_の動作に推奨される要件をインストールが満たしているか確認する。
4. `ログをダウンロード`ボタンでログファイルをダウンロードし、テストレポートに**この情報を添付する**。
5. 左側のサイドバーでTainacanをクリックする：

- [x] ホーム画面の読み込み時間を確認する；
- [x] ページのすべての要素が正しく表示されているか確認する；
- [x] 画面の読み込み時間または要素の表示に大きな変化や誤りがないか報告するため、以下のプロセスを完了した後にこれらの点をもう一度確認する。

これが完了したら、より詳しくテストしたいトピックを選択します：

<div style="column-count: 2; column-width: 250px;">

- [コレクション](/ja/testing-collections)
- [タクソノミー](/ja/testing-taxonomies)
- [メタデータ](/ja/testing-metadata)
- [フィルター](/ja/testing-filters)
- [アイテム](/ja/testing-items)
- [ファセット検索](/ja/testing-search)
- [インポーター](/ja/testing-importers)
- [エクスポーター](/ja/testing-exporters)
- [権限](/ja/testing-capabilities)
- [Gutenbergブロック](/ja/testing-gutenberg-blocks)
- [アイテム投稿](/ja/testing-item-submission)

</div>