# PS Live デブコン祭り：Reactの開発環境をdevcontainerで作る

pullしてdevcontainerで起動すれば実行できます。

## プロジェクト要件

- Nodeバージョン：20.10.0
- パッケージ管理ツール：npm
- ビルドツール：Vite
- プロジェクト：React + Typescirpt

## 資料

発表資料：assets/PS Live　デブコン祭り-React.pdf

- [環境作成：Reactプロジェクトの作成](https://gist.github.com/Ryunosuke-Tanaka-sti/b5dcab4d96455e9021f05b156ff37d0b)
- [改善](https://gist.github.com/Ryunosuke-Tanaka-sti/ce76a7bfbc82485dbeb7d4de2261d6ef)
  - 改善①Volume Trickを使用してコンテナ内に収める
  - 改善②：Docker build時のキャッシュを活用
- [環境作成：devcontainerで立ちあげる](https://gist.github.com/Ryunosuke-Tanaka-sti/fee59072fe5c9e3a1483315d02651e96)

## ディレクトリ構造

```txt
.
├── .devcontainer
│   ├── Dockerfile              
│   └── devcontainer.json       // devcontainer設定ファイル
├── frontend                    // フロントエンドプロジェクト
├── .dockerignore
├── docker-compose.yml
└── README.md
```
