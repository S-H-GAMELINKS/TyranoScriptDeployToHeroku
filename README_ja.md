# TyranoScriptDeployToHeroku
## 概要

ティラノスクリプトやティラノビルダーで作ったブラウザゲームを無料で使えるサーバ：Herokuにデプロイするためのものです。

## 使い方

まず、cloneしてローカルに保存します

```
git clone https://github.com/S-H-GAMELINKS/TyranoScriptDeployToHeroku.git
```

clone が終わったら `public` というフォルダを作成します。

```
mkdir public
```

次に、`public`内にブラウザゲーム向けにエクスポートしたティラノスクリプトやティラノビルダーで作ったゲームを配置します。
その後、git commit します

```
git commit -am "Deploy to Heroku, for TyranoScript!"
```

Heroku にアプリケーションを下記のコマンドで作成します。APP_NAME には 好きなアプリケーション名を使用してください。

```
heroku apps:create -a APP_NAME
```

下記コマンドで、Heroku のアプリケーションとローカルのリポジトリを接続します。

```
heroku git:remote -a APP_NAME
```

あとは、push するだけです。

```
git push heroku master
```

デプロイしたゲームをブラウザで確認する場合、以下のコマンドで確認できます。

```
heroku open -a APP_NAME
```

## 参考資料

[HerokuにRackでdeployする(初級編:静的HTMLページ)](https://qiita.com/higuma/items/9baac9e97eeb862ef64e)
