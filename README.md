# My Music Player（GitHub Pages / Notion埋め込み）

## ファイル構成

- `index.html`：プレイヤー本体（HTML・CSSを内包）。アルバム名・アーティスト名・レコード会社名は指定内容に設定済みです。
- `assets/cover.jpg`：ご自身のアートカバー
- `assets/song.mp3`：ご自身のMP3

## 1. ファイルを準備する

1. `assets` フォルダに、アートカバーを `cover.jpg` という名前で保存します。
2. MP3を `song.mp3` という名前で保存します。
3. `index.html` を開き、`YOUR SONG TITLE`、`YOUR ARTIST NAME`、サンプル歌詞を実際の内容に置き換えます。
4. ファイル名を変えた場合は、HTML内の `assets/cover.jpg` と `assets/song.mp3` も変更してください。

## 2. GitHubにアップロードする

1. https://github.com/new を開き、新しいリポジトリを作ります（例：`music-player`）。
2. 公開する場合は `Public` を選び、`Create repository` を押します。
3. リポジトリで `Add file` → `Upload files` を選びます。
4. `index.html` と `assets` フォルダ内の `cover.jpg`、`song.mp3` をアップロードし、`Commit changes` で保存します。
5. フォルダ構成が次のようになっていることを確認します。

   ```
   music-player/
   ├── index.html
   └── assets/
       ├── cover.jpg
       └── song.mp3
   ```

## 3. GitHub Pagesを有効にする

1. リポジトリの `Settings` → `Pages` を開きます。
2. `Build and deployment` の `Source` を `Deploy from a branch` にします。
3. Branch を `main`、フォルダを `/(root)` にして保存します。
4. 公開処理が終わるまで数分待ち、Pages画面に表示されるURLを開きます。
5. 画像、再生、歌詞スクロールが動くことを確認します。

URLは通常 `https://ユーザー名.github.io/music-player/` の形式ですが、必ずGitHubが表示したURLを使ってください。

## 4. Notionに埋め込む

1. Notionのページで `/embed` と入力し、埋め込みブロックを追加します。
2. GitHub Pagesの公開URLを貼り付けて確定します。
3. 表示されない場合は、まず公開URLをブラウザで直接開けるか確認してください。

## 仕様

- PCではアートカバーと曲情報を左側、歌詞を右側に表示します。
- スマホでは歌詞がプレイヤーの下に移動します。
- 歌詞は全文を表示し、歌詞欄だけを独立してスクロールできます。
- 歌詞は再生時間と同期しません。
- 再生UIはブラウザ標準の音声コントロールです。

## 注意

- GitHubのPublicリポジトリにアップロードした音源・画像・歌詞は公開状態になります。公開してよい素材だけを使ってください。
- GitHubの通常のGit経由アップロードでは、1ファイルが100 MiBを超えると扱えません。大きなMP3は外部ストレージなどを検討してください。
- Notionの埋め込み表示は、ブラウザやNotion側の仕様・制限により見え方が異なる場合があります。
