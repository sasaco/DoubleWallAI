# フォルダ

- src : 機械学習のソースコード保存フォルダ
- data : 機械学習用 csv データ保存フォルダ
- docs : 論文

# 論文執筆には　Vivliostyle CLI　を使います

https://vivliostyle.org/viewer/#src=https://sasaco.github.io/DoubleWallAI/

- コマンドラインから CSS 組版をして表示します。PDF に出力できます。

## インストール方法

事前に Node.js のインストールが必要です。
npm パッケージからインストールできます。

```
$ npm install -g @vivliostyle/cli
```

### プレビューの表示

docsフォルダをカレントフォルダにした状態で、 
preview コマンドを指定すると、閲覧ができます。

```
DoubleWallAI\docs> vivliostyle preview index.html
```
![](https://vivliostyle.org/assets/projects/screenshot-cli.png)

Vivliostyle CLI について詳しくは [Vivliostyle CLI ユーザーガイド](https://docs.vivliostyle.org/#/ja/vivliostyle-cli) を参照してください。


## HTMLからPDFを作成する

ターミナルのコマンドラインから、build コマンドで HTML ファイルを指定すると、CSS 組版した PDFファイルを出力できます。

```
DoubleWallAI\docs> vivliostyle build index.html
```