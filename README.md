# okimurak.github.io

![Publish Github Page](https://github.com/okimurak/okimurak.github.io/workflows/Publish%20Github%20Page/badge.svg)

<https://okimurak.github.io> のソース

[Hugo](https://gohugo.io/) とテンプレートを使い、GithubPages でホスティングしています

## Requirement

- Docker
- docker-compose

## Launch

- Repository を Clone

```bash
git clone https://github.com/okimurak/okimurak.github.io
docker-compose up -d
```

- Theme を Clone

```bash
git clone https://github.com/lxndrblz/anatole.git themes/anatole
```

- Docker compose で起動

```bash
docker-compose up -d
```

- ローカル(http:/localhost:1313)にブラウザからアクセス

## Theme

`./themes`　以下に配置して使う

- [Anatole | Hugo Themes](https://themes.gohugo.io/anatole/)

## Github Actions

Github Action を使って Github Pages にデプロイを行っている

- [こちら](https://github.com/peaceiris/actions-gh-pages#%EF%B8%8F-create-ssh-deploy-key)を参考に、リポジトリの Secret に`ACTIONS_DEPLOY_KEY` を追加する

## Reference

- https://github.com/iganari/iganari.github.io
