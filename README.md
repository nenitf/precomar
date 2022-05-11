# precomar

[![emojicom](https://img.shields.io/badge/emojicom-%F0%9F%90%9B%20%F0%9F%86%95%20%F0%9F%92%AF%20%F0%9F%91%AE%20%F0%9F%86%98%20%F0%9F%92%A4-%23fff)](http://neni.dev/emojicom) [![CI](https://github.com/nenitf/precomar/actions/workflows/ci.yml/badge.svg)](https://github.com/nenitf/precomar/actions/workflows/ci.yml)

Análise OPEA

<!--
## Utilização

1. Baixe o [projeto](https://github.com/nenitf/precomar/releases/latest)
2. Execute ``./precomar``

> Análises sem relatório com ``./precomar -14.900946 -40.903358``
-->

## Desenvolvimento

> [Estrutura](https://github.com/bnkamalesh/goapp)

### Primeira inicialização

```sh
docker-compose up -d
docker-compose exec app go mod tidy
```

### Demais inicializações

```sh
docker-compose up -d
```

> Pare com ``docker-compose down``

### Teste

```sh
docker-compose exec app go test ./...
#docker-compose exec app go test ./internal/precomar
#docker-compose exec app go test ./internal/precomar/domainx/pkgname_test.go
#docker-compose exec app go test ./internal/precomar -run "regexOfTest$"
```

## Linting

```sh
docker-compose exec app go fmt ./...
```
