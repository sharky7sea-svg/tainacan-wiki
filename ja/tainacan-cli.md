# Tainacan CLI

WP-CLI (https://wp-cli.org/)はWordPressのコマンドラインインターフェースです。Webブラウザーを使わずに、プラグインの更新、マルチサイトインストールの設定など、さまざまな操作を行えます。

## WP-CLIコマンド
Tainacanでは、次のWP-CLIコマンドがサポートされています：

```
    wp tainacan garbage-collector
    wp tainacan move-attachments-to-items-folder
    wp tainacan collection
    wp tainacan index-content
    wp tainacan control-metadata
```


### wp tainacan garbage-collector
未使用のファイルとデータベースエントリを削除して、Tainacanのインストールをクリーンアップします。
#### オプション：
| オプション           | 説明 |
|-------------------|-------------|
|--run              | デフォルトでは、このコマンドはゴミを探してレポートを出力するだけで、何も削除しません。実際にゴミを削除する場合は、--runを渡します。 |
|--deep             | ゴミを見つけるための、より積極的なアプローチです。場合によっては、Webサイトの他の部分に関連するものを削除する可能性があります。現在、deepモードでは、Tainacan経由でアップロードされたかどうかに関係なく、親IDが壊れているすべての添付ファイルを削除します。 |
|--skip-attachments | 孤立した未使用の添付ファイルを探さないようにします。 |
|--skip-items       | 孤立した未使用のアイテムを探さないようにします。 |
|--skip-taxonomies  | 孤立した未使用のタクソノミーを探さないようにします。 |
|--skip-metadata    | 孤立した未使用のメタデータを探さないようにします。 |
|--skip-transients  | Tainacanの一時データを探さないようにします。 |
|--yes              | 実行前の確認を省略します。 |

例：
```
wp tainacan garbage-collector --run --deep --yes
```


### wp tainacan move-attachments-to-items-folder
アイテムのドキュメントと添付ファイルを、`$collection_id/$item_id`のディレクトリ構造へ移動します。
これは、この構造が実装されたTainacanバージョン0.11より前に作成されたインストールの構造を更新するためだけに使用します。

#### オプション：
| オプション    | 説明 |
|------------|-------------|
|--dry-run   | 添付ファイルを探しますが移動せず、レポートだけを出力します。 |

例：
```
wp tainacan index-content --collection=all
```

### wp tainacan collection list
コレクションの一覧を表示します。

### wp tainacan collection clean
特定のコレクションのアイテムを削除します。

#### オプション：
| オプション        | 説明 |
|----------------|-------------|
|<collection_id> | アイテムを削除するコレクションを指定します。 |
|--permanently   | ゴミ箱を経由せず、アイテムを完全に削除します。 |
|--dry-run       | 削除するアイテムの合計数だけを数え、レポートを出力します。 |


例：
```
wp tainacan collection clean 1201 --permanently
```


### wp tainacan index-content
ドキュメントの内容をインデックス化します。

#### オプション：
| オプション             | 説明 |
|---------------------|-------------|
|--collection=<value> | <value> アイテムのドキュメント内容をインデックス化する特定のコレクションID、またはすべてのコレクションを対象とする場合は'all'。 |
|--dry-run            | インデックス化するアイテムの合計数だけを数え、レポートを出力します。 |


### wp tainacan control-metadata
メタデータの制御値を再計算します。

#### オプション：
| オプション              | 説明 |
|----------------------|-------------|
|--collection=<value> | <value> 制御メタデータを再計算する特定のコレクションID、またはすべてのコレクションを対象とする場合は'all'。 |
|--dry-run             | 再計算するアイテムの合計数だけを数え、レポートを出力します。 |
|--recreate-control-metadata-definitions | 制御メタデータのコレクション定義を再作成します。 |

例：
```
wp tainacan control-metadata --collection=all --recreate-control-metadata-definitions
```
