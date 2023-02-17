# pycon.jp.2023.teaser

## 初期設定

nvmを利用する場合は、以下のコマンドを初回に実行してください。

```
$ nvm install
```

その他の環境の場合は、`Node.js 14.16.0`に合わせた環境を準備ください

## 開発について

devブランチにマージすると、自動的に開発環境にデプロイされます
mainブランチにマージすると、自動的に本番環境にデプロイされます
ただし、masterへのマージは必ず一人の承認が必要です(間違ってデプロイされることを防ぐため)

devブランチには、原則直接プッシュせず、プルリクを作成してください
devへのプルリクはセルフマージしてもらって大丈夫です

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

### Tips

- proxy配下でのyarn install 方法

```bash
 yarn config set proxy http://example.com:port -g
```

- hash check error の回避方法

```bash
yarn --update-checksums
```
