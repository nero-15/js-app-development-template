# js-app-development-template
javascript アプリ開発時のテンプレート

## 概要
webpack等を用いてすぐに開発が始められる環境を構築するためのフローをまとめています。

## 環境
- node v14.16.0

## やり方

1. 初期設定
```
npm init -y
```

2. 該当パッケージインストール
```
npm install --save-dev webpack webpack-cli html-webpack-plugin express webpack-dev-middleware
```

3. 必要なファイルを作成
```
touch webpack.config.js
touch server.js
mkdir src
touch src/app.js
```

4. 各設定ファイルにコード追加

- webpack.config.js
- server.js
- src/app.js

ソースコードの内容コピー＆ペースト。その後必要に応じてカスタマイズ。

5. package.json に script 追加
```
"scripts": {
	"build": "webpack --config webpack.config.js",
	"server": "node server.js",
}
```

6. ビルド実行
```
npm run build
```

7. サーバ起動
```
npm run server
```
http://localhost:3000/

8. アプリ開発を始めよう！！
