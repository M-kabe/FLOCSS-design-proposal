#CSSのガイドライン

- ファイル・ディレクトリ構成


## ファイル・ディレクトリ構成
ファイル構成はFLOCSSをベースにします。FLOCSSの詳しい説明は[こちら](https://github.com/hiloki/flocss)

```
.
├── foundation/
│   ├── _reset.scss
│   ├── _base.scss
│   ├── _variable.scss
│   ├── _mixin.scss
├── layout/
│   ├── _header.scss
│   ├── _main.scss
│   ├── _sidebar.scss
│   ├── _footer.scss
├── object/
│   ├── component/
│   │   ├──
│   │   ├──
│   │   ├──
│   ├── project/
│   │   ├──
│   │   ├──
│   │   ├──
│   ├── utility
│   │   ├──
│   │   ├──
│   │   ├──
└── style.scss
```

全てのファイルはstyle.scssとして統合します。

* fundation  → サイト全体のデフォルトスタイルを管理する。
  * variable.scssは、サイト全体で使える変数
  * mixin.scss サイト全体で使えるmixin管理

* layout  → 各ページを構成するサイト全体で共通したエリアを管理
  * l-header.scss
  * l-main.scss
  * l-sidebar.scss
  * l-footer.scss

* object  → サイト全体で再利用できるパターンをもつモジュールを管理
  * component  → 小さな単位のモジュールを管理（ボタンなど）
    *  例 c-button.scss
    *  例 c-grid.scss

  * project  → いくつかのcomponentと、他の要素によって構成される大きい単位のモジュールを管理
    *  例 p-card.scss
    *  例 p-profile.scss

  * utility  → componentとprojectのパターンで解決できないスタイル、または調整のための便利クラスなどを管理


## ファイル・ディレクトリ構成
