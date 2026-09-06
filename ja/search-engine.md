> [!NOTE]
> このページの原文は*ブラジルポルトガル語*で提供されています。

# 検索エンジン

[ファセット検索](/dev/faceted-search.md)では、特定のメタデータによってアイテムを絞り込めます。これに加えて、Tainacanでは自由なテキスト検索も利用できます。

デフォルトでは、自由なテキスト検索を使用すると、WordPressはタイトル（post_title）と説明（post_content）の中だけを検索します。この方法には明らかな制限があるため、ここではTainacanがこの制限に対処するために採用している方法について説明します。

この問題を解決する魔法の方法はありません。場合によっては、特に小規模なリポジトリでは、メタデータとタクソノミーの関係を含め、WordPressが投稿を検索する方法を少し変更するだけで、ユーザーが求める結果を得られる可能性があります。また、リポジトリの管理者は、ElasticSearchやSolrのような、より高度な解決策を使って、ユーザーがすべてのコンテンツを対象にテキスト検索できるようにしたい場合もあります。

中間的な方法として、インデックステーブル（index tables）を作成し、文字列をトークン化（tokenizing strings）することもできます。これにより、関連性に基づいて結果を並べ替えることさえ可能になります（これを行う有料のWordPressプラグインは少なくとも1つあります）。

これらすべての選択肢を考慮し、ここではWordPressのWP_Queryオブジェクトによって構築されたSQLクエリをフィルターし、メタデータとタクソノミーの値を対象とした検索を追加します。この方法は、プラグイン「[Search Everything](https://wordpress.org/plugins/search-everything/)」が採用しているものと同じです。

この方法では、検索、特に自由なキーワード検索のフィールドが遅くなる可能性があります。

この変更を無効にしてWordPressのデフォルトの動作（タイトルと説明だけを検索）に戻したい場合は、`wp-config.php`ファイルに次の行を追加します。別の検索プラグインを使用する場合は、競合の可能性を避けるため、これを行うことをおすすめします。

```
define('TAINACAN_DISABLE_DEFAULT_SEARCH_ENGINE', true);
```

現在、私たちは[ElasticPress](https://wordpress.org/plugins/elasticpress/)プラグインとの互換性向上に取り組んでいます。これは[version 0.9](https://tainacan.org/blog/2019/05/20/tainacan-beta-0-9-elastic-search-new-gutenberg-block-and-importers/)以降、完全に機能しています。
*注：対応しているElasticSearchのバージョン：elasticsearch 6.1.0+*

リポジトリが非常に大きくなった場合は、より堅牢なインフラストラクチャが必要になる可能性があり、ElasticSearchの使用をおすすめします。

しかし、WordPressの「やり方」に沿って開発することを重視しており、Tainacanの検索は検索にネイティブの「WP_Query」クラスを使用しているため、このクラスを使う検索プラグインであればTainacanでも動作するはずです。ぜひWordPress用の別の検索プラグインも試して、どの程度うまく動作したか教えてください！
