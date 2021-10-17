# 2021-club-journal.github.io

## セットアップ方法
nodejsとnpmをお使いの環境でインストールし、下記のコマンドを入力してください。

```shell
    npm -g install honkit \
        gitbook-plugin-expand-active-chapter \
        gitbook-plugin-collapsible-chapters  \
        gitbook-plugin-prism  \
        gitbook-plugin-copy-code-button \
        gitbook-plugin-hide-published-with  \
        gitbook-plugin-anchors  \
        gitbook-plugin-intopic-toc  \
        gitbook-plugin-back-to-top-button  \
        gitbook-plugin-hints \
        gitbook-plugin-git-author  --save-dev
```

## セットアップ用Makefile
セットアップの時に使えるMakefileを作りました。
bash向けに書いたので他のシェルをお使いの方は読み替えてください。
実行した後は
```shell
 source ~/.bash_profile
```
をシェルで動かしてください。
[【備忘録】npm -g install に失敗する](https://qiita.com/NaokiIshimura/items/cc07441939b226e779c6)を参考にしてこのMakefileを書きました。
```shell
make run
```
ディレクトリに移動して上記コマンドで実際にテストできます。
```Makefile
setup:
	sudo apt install -y nodejs npm
	mkdir ~/.npm-global
	npm config set prefix '~/.npm-global'
	echo ' export PATH=~/.npm-global/bin:$PATH' >> ~/.bash_profile
	export PATH=~/.npm-global/bin:$PATH
	npm -g install honkit gitbook-plugin-expand-active-chapter gitbook-plugin-collapsible-chapters  gitbook-plugin-prism  gitbook-plugin-copy-code-button gitbook-plugin-hide-published-with  gitbook-plugin-anchors  gitbook-plugin-intopic-toc  gitbook-plugin-back-to-top-button  gitbook-plugin-hints gitbook-plugin-git-author  --save-dev
run:
	honkit serve
```

## 使用しているソフトウェア
[Node.js](https://nodejs.org/ja/)はJavascriptの実行環境です。<br>
[npm](https://www.npmjs.com/)はNode.jsのパッケージマネージャーです。<br>
[honkit](https://github.com/honkit/honkit)は[Gitbook](https://github.com/GitbookIO/gitbook)のフォークで、マークダウンで書ける、ドキュメント作成ツールです。

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