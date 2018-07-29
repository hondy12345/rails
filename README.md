# RoR_EC
[![CircleCI](https://circleci.com/gh/hondadadadada/rails/tree/master.svg?style=svg)](https://circleci.com/gh/hondadadadada/rails/tree/master)

Ruby on Railsを利用したECサイトの構築プロジェクトです。

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
