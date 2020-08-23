# mygration
flywayを使用した際に色々と調べたことの備忘録。

## mygrationとは
システムまたはデータ資産の移行のこと。
なにを指すかはケースバイケースバイだが、端的に言うと移行作業全般のこと。

### DBマイグレーション
DBに保存されているデータを保持したまま、テーブルの作成やカラムの変更などを行うための機能。
データベースを削除した際にデータも消えてしまうと言う事態を回避する。

### flyway
JVM上で動作するDBマイグレーションツール。
アプリケーションの成長（？）とともにデータベースの構成やカラム数などが増えていくことが普通。そこで、データベースの状態を保存しバージョン管理できると嬉しい。
ので、FlyWayを使用する。

現在のDBの状態（現在のテーブル構成、カラム構成にいたるまでにどういう作成・変更等があったかの情報）に関する情報を一箇所で管理し、再現する。
データーベースの状態をバージョン管理すると言うこと。

* DBの定義やその変更に関する情報を一箇所で管理する
* その情報に基づき最新のDBの状態を自動で再現する
↑こんなことをやってくれる

命名ルールがある↓

    V<バージョン>__<任意の名前>.sql
    


**********************************************************************
参考：
* マイグレーションとは
https://www.sophia-it.com/content/%E3%83%9E%E3%82%A4%E3%82%B0%E3%83%AC%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3
* DBマイグレーションとは
https://densan-labs.net/tech/codefirst/migration.html
* FlyWayについて
https://qiita.com/rubytomato@github/items/d1746585451ff0ba917c
* FlyWay Documentation
https://flywaydb.org/documentation/
