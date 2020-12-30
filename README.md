# Electron Sample - コード署名（macOS）
macOSでコード署名を行うのに必要なファイルをまとめたサンプルです。

## 解説ページ
* [[Electron] macOS用アプリに「コード署名」と「公証」を行う](https://blog.katsubemakito.net/nodejs/electron/codesigning-macos)

## 重要
このリポジトリには環境変数の設定を行うための「**.env**」を登録していますが、実際に開発する場合には<strong style="color:red">絶対に</strong>含めないでください。

## 準備
Gitでリポジトリを取得します。
```shellsession
$ git clone https://github.com/katsube/electron-sample-signcode-mac.git
```

Node.jsがインストールされている環境で以下のコマンドを実行し、必要なライブラリを取得します。
```shellsession
$ cd electron-sample-signcode-mac
$ npm install
```

## 実行方法
以下でプレビューを行います。
```shellsession
$ npm start
```

「[解説ページ](https://blog.katsubemakito.net/nodejs/electron/codesigning-macos)」で行った設定を一通り実行してください。その上で以下のビルド用コマンドを叩くと、各OS用のインストーラーが作成されます。
```shellsession
$ npm run build-win
$ npm run build-mac
```

