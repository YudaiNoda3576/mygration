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
