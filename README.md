# LEMP_test

## １．概要
以前作成した「dockerでLAMP環境+LocalStackで疑似AWS環境を作成する」プロジェクトをもとに、LAMP環境をLEMP環境へ変更することを目的としたリポジトリです。
フレームワークとしてLaravelを使用するようになっています。

## ２．動作環境
以下の環境での動作を確認済みです。
* **OS**: windows 11 (25H2)
* **Docker**: version 28.5.2
* **Docker Compose**: version 2.40.3

## ３．セットアップ手順
1) リポジトリをクローン
2) `.env.example`ファイルを編集し、`.env`ファイルに名前を変更（4.を参照）
3) docker composeでコンテナを一括起動<br>
    以下のコマンドをルートディレクトリで実行してください。

     ```bash
     docker compose up -d
     ```

4) 動作確認方法<br>
     ブラウザで以下のURLにアクセスしてください。<br>
     **Laravel**: http://localhost:8081 <br>
     
## ４．環境変数の設定
プロジェクトのルートに`.env`ファイルを作成し、以下の内容を設定してください。

```text
# MySQL設定
DB_ROOT_PASSWORD=root 
DB_NAME=test_db  # 任意
DB_USER=test_user  # 任意
DB_PASSWORD=test_password  #任意のパスワードを設定

```
## ５．使い方/サンプル

## ６．構成図

dockerを使用した構成のため、ホストOSに影響を与えずに仮想環境の構築が可能です。

## ７．よくある質問・トラブルシューティング

## ８．TODO/今後やりたいこと

## ９．更新履歴
* **2026-03-23**:　リポジトリ作成

## ライセンス
このプロジェクトは[MITライセンス](LICENSE)のもとで公開されています。