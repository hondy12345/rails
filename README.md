# RoR_EC
[![CircleCI](https://circleci.com/gh/hondadadadada/rails/tree/master.svg?style=svg)](https://circleci.com/gh/hondadadadada/rails/tree/master)

Ruby on Railsを利用したECサイトの構築プロジェクトです。

# 機能
## フロント
### 商品情報画面
- /products/{id}
### カート画面
- /cart
### 購入確認画面
- /shopping/confirm
### 購入完了画面
- /shopping/complete
### 会員登録画面
- /register
### 会員ログイン画面
- /login
### マイページ
- /mypage
## 管理画面
### 管理者ログイン画面
- /admin/login
### SHOP管理
#### 基本設定
- /admin/shop_info
- 店名/メールアドレス/住所の設定を行う
#### 配送業者管理
- /admin/deliv_companies
- 配送業者の情報/都道府県ごとの送料の設定を行う
#### 支払い方法管理
- /admin/payments
- 支払い方法の情報/手数料を設定を行う
#### 消費税管理
- /admin/taxes
- 消費税の設定を行う
#### ユーザ管理
- 管理画面のユーザの管理を行う
### 商品系管理
#### 商品カテゴリ管理
- /admin/product_categories
- 商品カテゴリ情報の設定を行う
#### 商品管理
- /admin/products
- 商品情報の設定を行う
#### 商品レビュー管理
- /admin/product_reviews
- 商品レビューの閲覧・非公開設定などを行う
### 受注系管理
#### 受注管理
- /admin/orders
- 受注情報の検索・受注情報の変更を行う
#### 受注ステータス管理
- /admin/order_statuses
- 受注ステータスの設定を行う
### 発送系管理
#### 発送管理
- /admin/delivs
- 発送処理を行う

# 動作環境
* OS
    * macOS High Sierra 10.13.5
* Ruby version
    * ruby 2.4.1p111 (2017-03-22 revision 58053) [x86_64-darwin17]
* MySQL version
    * mysql  Ver 8.0.11 for osx10.13 on x86_64 (Homebrew)

# 利用技術
* テストツール
    * RSpec
    * CircleCI
* HTMLテンプレートエンジン
    * Slim

# 利用技術の採用理由
## Slim
[公式](http://slim-lang.com/index.html)

参考：[Railsのテンプレートエンジンの比較 erb vs slim vs haml](http://ruby-rails.hatenadiary.com/entry/20141001/1412169453)

Hamlと比較した際、少し指が届きづらい"%"を頻繁に打つのが少し面倒なのでSlimにしました。

## sorcery
[公式](https://github.com/Sorcery/sorcery)

参考：[Rails でアカウントロジックを扱うなら sorcery が良いかも](https://qiita.com/ltcmdr927/items/90ba8b924ad65d773625)

deviceよりsorceryのほうが楽だと聞いたので。
四苦八苦しましたが公式に載っている[Simple Password Authentication](https://github.com/Sorcery/sorcery/wiki/Simple-Password-Authentication)通りにやるとすんなりでした。

# 主なファイル・ディレクトリ構造
|ファイル・ディレクトリ名|説明|
|---|---|
|/Gemfile|Bundlerの設定ファイル|
|/Gemfile.lock|Gemfileを元に生成される。開発環境・運用環境で同じgemをインストールするためのファイル|
|/Rakefile|rakeコマンドで実行できるタスクを定義するファイル|
|/app/assets/|js/css/画像などを格納するディレクトリ|
|/app/controllers/|コントローラクラスを格納するディレクトリ|
|/app/controllers/application_controller.rb|共通のコントローラ|
|/app/helpers/|ヘルパを格納するディレクトリ|
|/app/models/|モデルクラスを格納するディレクトリ|
|/app/views/|viewファイル(slim)を格納するディレクトリ|
|/config/|設定ファイルを格納するディレクトリ|
|/db/migrate/|マイグレーションファイルを格納するディレクトリ|
|/public/|公開されるファイルを格納するディレクトリ|
|/spec/|RSpecで利用するテスト用クラスを格納するディレクトリ|
