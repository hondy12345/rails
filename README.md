# RoR_EC
[![CircleCI](https://circleci.com/gh/hondadadadada/rails/tree/master.svg?style=svg)](https://circleci.com/gh/hondadadadada/rails/tree/master)

Ruby on Railsを利用したECサイトの構築プロジェクトです。

# 機能
## フロント
### 商品情報画面
### カート画面
### マイページ
### 購入確認画面
### 購入完了画面
## 管理画面
### SHOP管理
#### 基本設定
- 店名/メールアドレス/住所の設定を行う
#### 配送業者管理
- 配送業者の情報/都道府県ごとの送料の設定を行う
#### 支払い方法管理
- 支払い方法の情報/手数料を設定を行う
### 商品系管理
#### 商品カテゴリ管理
- 商品カテゴリ情報の設定を行う
#### 商品管理
- 商品情報の設定を行う
#### 商品レビュー管理
- 商品レビューの閲覧・非公開設定などを行う
### 受注系管理
#### 受注管理
- 受注情報の検索・受注情報の変更を行う
#### 受注ステータス管理
- 受注ステータスの設定を行う
### 発送系管理
#### 発送管理
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
参考：[Railsのテンプレートエンジンの比較 erb vs slim vs haml](http://ruby-rails.hatenadiary.com/entry/20141001/1412169453)

Hamlと比較した際、少し指が届きづらい"%"を頻繁に打つのが少し面倒なのでSlimにしました。
