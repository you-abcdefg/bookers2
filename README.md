# Bookers2

## 概要
ユーザー登録・ログイン機能（Devise）付きの書籍管理Webアプリです。ユーザーは書籍の投稿・編集・削除ができ、プロフィール画像や自己紹介も設定できます。

## 主な機能
- ユーザー登録・ログイン（Devise）
- 書籍（Book）のCRUD
- ユーザーのプロフィール編集・画像アップロード
- 他ユーザーの書籍閲覧

## 動作環境
- Ruby 3.1.2
- Rails 6.1.7
- SQLite3

## セットアップ手順
1. 必要なgemをインストール
	```
	bundle install
	```
2. データベース作成・マイグレーション
	```
	rails db:create
	rails db:migrate
	```
3. サーバー起動
	```
	rails server
	```
4. ブラウザで `http://localhost:3000` にアクセス

## フォルダ構成
- app/models: User, Bookモデル
- app/controllers: users, books, homesコントローラ
- app/views: 各種画面（ユーザー、書籍、ホーム等）

## 備考
- Deviseによる認証機能
- プロフィール画像はActiveStorageで管理
- 書籍本文は200文字まで
