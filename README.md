# devcontainer-go

Go devcontainer template

## 必要要件

- Docker
- Visual Studio Code
- Dev Containers 拡張機能

## 起動方法

### 1. Dev Containerで開く

```bash
# VS Codeでプロジェクトを開く
code .
```

VS Codeでコマンドパレット（`Cmd+Shift+P` / `Ctrl+Shift+P`）を開き、
`Dev Containers: Reopen in Container` を選択してください。

### 2. アプリケーションの実行

```bash
# プログラムを実行
go run main.go
```

### 3. ビルドして実行

```bash
# バイナリをビルド
go build -o app main.go

# ビルドしたバイナリを実行
./app
```

## 開発

### 依存パッケージの追加

```bash
# パッケージを追加
go get <package-name>

# go.modを整理
go mod tidy
```

### フォーマット

```bash
# コードをフォーマット
go fmt ./...
```

### テストの実行

```bash
# すべてのテストを実行
go test ./...

# カバレッジ付きでテスト
go test -cover ./...
```

## 含まれているツール

このDev Containerには以下のツールがプリインストールされています:

- Go (最新版)
- Git
- Node.js & npm
- 各種Goユーティリティ

## プロジェクト構造

```
.
├── .devcontainer/       # Dev Container設定
├── main.go             # メインアプリケーション
└── README.md           # このファイル
```
