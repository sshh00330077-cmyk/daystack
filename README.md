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
| Frontend | Next.js 16 / TypeScript / Tailwind CSS |
| Backend | Go / Gin |
| Database | PostgreSQL |
| インフラ | (デプロイ先を書く) |


---

## ディレクトリ構成

```
daystack/
├── frontend/
│   ├── app/
│   │   ├── page.tsx          # トップページ (localhost:3000)
│   │   ├── layout.tsx        # 全ページ共通の外枠
│   │   ├── globals.css       # 全体のCSS
│   │   ├── schedule/
│   │   │   └── page.tsx      # スケジュールページ (localhost:3000/schedule)
│   │   ├── tasks/
│   │   │   └── page.tsx      # タスクページ (localhost:3000/tasks)
│   │   └── stats/
│   │       └── page.tsx      # 達成率ページ (localhost:3000/stats)
│   ├── public/
│   └── package.json
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



## AIとの開発ルール

- 作者はWeb開発ほぼ未経験。コードを書くだけでなく「なぜそうするか」を必ず説明すること
- 知らない概念が出たら都度解説する
- コマンドは自分で打ちたいので、実行せず教えるだけにする

### 今日話した内容メモ

- `npm run dev` = TypeScript/JSXをブラウザが読めるHTMLに変換するサーバーを起動するコマンド
- `localhost:3000` = 自分のPCで動いているサーバーのアドレス（3000はポート番号）
- Next.jsはフォルダ＝URLになる（`app/tasks/page.tsx` → `localhost:3000/tasks`）
- `node_modules/` は触らない、`app/` フォルダの中だけ触る
- 毎回の開発: `cd frontend` → `npm run dev` → コードを書く → git commit/push

---

## 開発の始め方

```powershell
cd frontend
npm run dev
```

ブラウザで http://localhost:3000 を開く。

---

## 今後の予定
- [x] Next.jsの環境構築
- [x] Next.jsのファイルを作成
- [ ] GoでAPI作成
- [ ] PostgreSQLのテーブル設計
- [ ] フロントとバックの繋ぎこみ
- [ ] Dockerとか使えるなら使いたい

---

## 作者

[SSHH](https://github.com/SSHH)