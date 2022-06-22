+++
title = "Installation"
description = ""
weight = 1
+++

## フロントエンド

[exdeck-frontend](https://github.com/EXDeck/exdeck-frontend)

### 必要要件

- Node.js Version Manager ([fnm](https://fnm.vercel.app/)を推奨)
- [Node.js](https://nodejs.org/) v17.9.0
- [pnpm](https://pnpm.io/)

### インストール

以下のコマンドを実行します。

```sh
git clone https://github.com/EXDeck/exdeck-frontend.git
cd exdeck-frontend
pnpm i
```

### 使い方

#### 開発用サーバーの起動

`src/.env.development.local` ファイルを作成します。

**HTTPS通信をする場合**は、`VITE_API_HTTPS`(HTTPS通信の実行フラグ) を `true` にし、`VITE_API_URL_HTTPS`(開発時にHTTPS通信を行うバックエンドのURL) を指定します。

**HTTP通信をする場合**は、`VITE_API_HTTPS`(HTTPS通信の実行フラグ) を `false` にし、`VITE_API_URL`(開発時にHTTP通信を行うバックエンドのURL) を指定します。

記入例は `src/.env.development.example` を参照してください。

その後、以下のコマンドを実行します。

```sh
pnpm dev
```

#### ビルド

`src/.env.production.local` ファイルを作成します。

**HTTPS通信をする場合**は、`VITE_API_HTTPS`(HTTPS通信の実行フラグ) を `true` にし、`VITE_API_URL_HTTPS`(HTTPS通信を行うバックエンドのURL) を指定します。

**HTTP通信をする場合**は、`VITE_API_HTTPS`(HTTPS通信の実行フラグ) を `false` にし、`VITE_API_URL`(HTTP通信を行うバックエンドのURL) を指定します。

記入例は `src/.env.production.example` を参照してください。

その後、以下のコマンドを実行します。

```sh
pnpm build
```

## バックエンド

[exdeck-backend](https://github.com/EXDeck/exdeck-backend)

### 必要要件

- Node.js Version Manager ([fnm](https://fnm.vercel.app/)を推奨)
- [Node.js](https://nodejs.org/) v18.3.0
- [Yarn](https://yarnpkg.com/)

### インストール

以下のコマンドを実行します。

```sh
git clone https://github.com/EXDeck/exdeck-backend.git
cd exdeck-backend
yarn install
```

### 使い方

#### 開発用サーバーの起動

以下のコマンドを実行します。

```sh
yarn dev
```

#### サーバーの起動

以下のコマンドを実行します。

```sh
yarn bs
```

#### ビルド

以下のコマンドを実行します。

```sh
yarn build
```
