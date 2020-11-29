# Flutter for web 環境構築

- Flutterのweb版での環境構築です。androidも頑張ればできます。
- dockerを使ったFlutterの環境構築なのでflutterdockと名付けています。
- 途中remote-containerを開かないといけないので動画を参考にしてください。

- 動画
   - [参考動画](https://gitlab.com/welcome-to-sodai/flutter-web/-/raw/master/video.mov?inline=false)

## FlutterDock

1. リポジトリをクローン

   ```
   git clone https://gitlab.com/welcome-to-sodai/flutter-web.git flutter_app/flutterdock
   ```

2. flutterdock階層で

   ```
   docker-compose build workspace
   ```

   いつも通り最初は長いです。wifi環境が良いときにやりましょう。

4. コンテナを構築、起動

   ```
   docker-compose up -d workspace
   ```

5. vscodeのremote-containerでworkspaceを開く

6. workspaceのbashに入りFlutterアプリを作成

   ```
   flutter create .
   ```

7. サーバーを起動

   ```
   flutter run
   ```

    そのうち右下にopenが出るのでクリックするとブラウザが開きます

## 使い方

- 始めるとき flutterdockの階層で
   ```bash
   docker-compose up -d workspace
   ```
- 終わるとき
   ```bash
   docker-compose down
   ```

## まとめ

- Flutter for webの環境構築ができた
- ひとまずFlutter触ってみたい！って人におすすめです
- データの永続化とかあんまりわからないです

## Next Step

- Flutterを勉強していくのみ!
- Sodai.でチュートリアル作ってくれる方募集中です...
