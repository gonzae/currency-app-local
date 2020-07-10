# currency-app-local

Just a local environment for [currency-converter-client](https://github.com/gonzae/currency-converter-client) & [exchange-api](https://github.com/gonzae/exchange-api).

## Before starting
Make sure you have already installed:
* Docker >= v19.03.8
* docker-compose >= v1.25.5

## Installation
Clone the following repos at same folder level:
* [currency-converter-client](https://github.com/gonzae/currency-converter-client)
* [exchange-api](https://github.com/gonzae/exchange-api)
* [currency-app-local (this one)](https://github.com/gonzae/currency-app-local)

Browse currency-app-local:
```
cd currency-app-local
```

In `docker-compose.yml`, replace `FIXER_ACCESS_KEY` placeholder with your [Fixer](https://fixer.io/) access key.

## Run
```
docker-compose build
docker-compose up -d
```

Log output (optional):
```
docker-compose logs -t -f client backend
```

Enjoy at http://localhost:3000/