# DayStack

> 意識高い系が使いたいようなサイト

---

## 概要

個人のスケジュール・タスク管理のために作成。
理想のスケジュールを曜日ごとに設定、タスク管理、今までの成果を可視化などが主な機能。

---

## 機能

- 曜日ごとの理想スケジュール設定（30分単位）
- タスク管理（追加・完了チェック）
- 達成率の可視化（グラフ）

---

## 技術スタック

| カテゴリ | 技術 |
| --- | ---|
| Frontend | Next.js |
| Backend | Go / Gin |
| Database | PostgreSQL |
| インフラ | (デプロイ先を書く) |


---

## ディレクトリ構成

```
calendar/
├── frontend/
├── backend/
└── README.md
```


---

## セットアップ

### 必要なもの


- Node.js v18以上
- Go v1.21以上
- postgreSQL


###　手順

```bash
# リポジトリをクローン
git clone https://github.com/ユーザー名/リポジトリ名.git
cd リポジトリ名
 
# フロントエンド
cd frontend
npm install
npm run dev
 
# バックエンド
cd ../backend
go mod tidy
go run main.go
```


---



## 今後の予定
- [ ] Next.jsの環境構築
- [ ] Next.jsのファイルを作成
- [ ] GoでAPI作成
- [ ] PostgreSQLのテーブル設計
- [ ] フロントとバックの繋ぎこみ
- [ ] Dockerとか使えるなら使いたい

---

## 作者

[SSHH](https://github.com/SSHH)