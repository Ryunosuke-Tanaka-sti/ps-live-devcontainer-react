# PS Live デブコン祭り：Reactの開発環境をdevcontainerで作る

pullしてdevcontainerで起動すれば実行できます。

## 資料

発表資料：assets/PS Live　デブコン祭り-React.pdf

- [環境作成：Reactプロジェクトの作成](https://gist.github.com/Ryunosuke-Tanaka-sti/b5dcab4d96455e9021f05b156ff37d0b)
- [環境作成：改善①Volume Trickを使用してコンテナ内に収める](https://gist.github.com/Ryunosuke-Tanaka-sti/ba79b6114fa72a2660ba9d104307e615)
- [環境作成：改善②：Docker build時のキャッシュを活用](https://gist.github.com/Ryunosuke-Tanaka-sti/b2bda3311f15851ad969de1e30a5680c)
- [起動確認](https://gist.github.com/Ryunosuke-Tanaka-sti/ce76a7bfbc82485dbeb7d4de2261d6ef)
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

## 要件

- Nodeバージョン：20.10.0
- パッケージ管理ツール：npm
- ビルドツール：Vite
- プロジェクト：React + Typescirpt
