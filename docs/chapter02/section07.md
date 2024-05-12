# Ionic の便利な機能

## Ionic CLI の便利なコマンド

### 開発のための処理が走る「Serve」

`ionic serve` を実行すると、Angular CLI のコマンドを自動的に呼び出して、次の処理を自動的に実行します。

1. ローカル開発サーバを起動する
2. プロジェクトで使われている SCSS と TypeScript をブラウザで表示できるようにするため、それぞれ トランスパイルする
3. 自動的にブラウザでローカル開発サーバにアクセスする
4. ローカルファイルの変更を監視して、変更があれば再ビルドして自動リロードを行う。

### 公式ドキュメントを立ち上げる「docs」

`ionic docs` を実行すると、ブラウザで公式ドキュメントが立ち上がります。  
なお、日本語ドキュメンテーションは、ドメインの `.com` を `.jp` に変更することでアクセスできます。

### 開発環境を表示する「info」

`ionic info` を実行すると、開発されている環境・設定を出力する機能があります。

### サードパーティライブラリを追加する「integrations」

`ionic integrations list` でサードパーティライブラリの一覧を表示できます。

```shell
$ ionic integrations list
name       | summary                                                                                                               | status
----------------------------------------------------------------------------------------------------------------------------------------------
capacitor  | Target native iOS and Android with Capacitor, Ionic's new native layer                                                | enabled
cordova    | Target native iOS and Android with Apache Cordova                                                                     | not added
enterprise | Ionic Enterprise Edition provides premier native solutions, UI, & support for companies building cross-platform apps. | not added
```

### CLI の設定値を登録する「config set」

`config set` を使うと、CLI の設定値を登録できます。

```shell
ionic config set --global npmClient yarn
```

## iOS / Android 別のデザインプレビュー

使えない？

## 圧倒的に各コードを減らしてくれる技術

### Web Components を使ったカスタム要素

Ionic は 「Web Components」という Web 標準の仕様を使って、オリジナルのタグを使えるようになる
カスタム要素でコンポーネントを作成しています。

