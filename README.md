# FLOCSS-design-proposal

## SCSSのコンパイル
黒い画面でやります。cloneした場合は、package.jsonが入っているので4以下の対応で大丈夫（なはず）

1. FLOCSS-design-proposalのディレクトリまで移動
2. `nmp init`でpackage.jsonを作成、エンター連打でok（package.jsonがある場合は不要）
3. node-sassをインストール
    - `npm install node-sass -D`
4. Sassの自動コンパイル
    - package.jsonファイル内のscriptsの値に以下追記
    - `"sass": "node-sass scss/ --output css/ --output-style expanded --watch --source-map true"`
5. npm-scriptsで定義したスクリプトを、以下のコマンドで実行
    - `npm run sass`

引用 [Sassを自動コンパイルする方法｜node-sassのインストール・利用例【npm】](https://blog-and-destroy.com/25933)
