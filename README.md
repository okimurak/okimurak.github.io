# okimurak.github.io

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

`./theme`　以下に配置して使う

- [Anatole | Hugo Themes](https://themes.gohugo.io/anatole/)

## Reference

- https://github.com/iganari/iganari.github.io
