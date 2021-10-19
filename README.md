# ここについて
このリポジトリは電算部の部誌のリポジトリです
## セットアップ方法
nodejsとnpmをお使いの環境でインストールし、下記のコマンドで、yarnをインストールしてください。

```shell
npm -g yarn
```
## 実行方法
実行方法はディレクトリに移動して、
```shell
yarn install
```
```shell
yarn honkit serve
```
すると、標準では、4000ポートでlocalhostにサーバーが立ち上がります。

## 使用しているソフトウェア
- [Node.js](https://nodejs.org/ja/)はJavascriptの実行環境です。<br>
- [npm](https://www.npmjs.com/)はNode.jsのパッケージマネージャーです。<br>
- [yarn](https://yarnpkg.com/)はNode.jsのパッケージマネージャーです。<br>
- [honkit](https://github.com/honkit/honkit)はマークダウン記法のドキュメント作成ツールです。

## 使用したプラグイン
- [gitbook-plugin-expand-active-chapter](https://www.npmjs.com/package/gitbook-plugin-expand-active-chapter)
- [gitbook-plugin-collapsible-chapters](https://www.npmjs.com/package/gitbook-plugin-collapsible-chapters)
- [gitbook-plugin-prism](https://www.npmjs.com/package/gitbook-plugin-prism)
- [gitbook-plugin-copy-code-button](https://www.npmjs.com/package/gitbook-plugin-copy-code-button)
- [gitbook-plugin-hide-published-with](https://www.npmjs.com/package/gitbook-plugin-hide-published-with)
- [gitbook-plugin-anchors](https://www.npmjs.com/package/gitbook-plugin-anchors)
- [gitbook-plugin-intopic-toc](https://www.npmjs.com/package/gitbook-plugin-intopic-toc)
- [gitbook-plugin-back-to-top-button](https://www.npmjs.com/package/gitbook-plugin-back-to-top-button)
- [gitbook-plugin-git-author](https://www.npmjs.com/package/gitbook-plugin-back-to-top-button)

## 参考にしたサイト
Github Actionsを書くときに参考にしたサイトです
- odanさんの[GitHub Actions で yarn install を爆速にしたい](https://zenn.dev/odan/scraps/81b2738864a908)
**node_modules 自体をキャッシュしてみる**を参考にしました。
- qualitia_cdevさんの[GitHub Actions の Workflow を高速化する](https://qiita.com/qualitia_cdev/items/407b0df9c0a0f0f45bbc)
**モジュールのインストールを高速化する**を参考にしました。
