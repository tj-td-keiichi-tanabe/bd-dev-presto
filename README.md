env_presto
====

Prestoの開発環境です。

## Description

## Demo

## VS. 

## Requirement

## Usage

```
# start service containers
docker-compose up -d --build mysql presto

# start controller container
docker-compose run --rm controller sh

# execute mysql query on controller container
mysql -u root -h 172.17.0.1 -e 'create database presto_sample'

# execute presto query on controller container
presto --server 172.17.0.1:8080 --catalog mysql --execute 'show schemas'
```

## Install

## Contribution

## Licence

[MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)

## Author

[canpok1](https://github.com/canpok1)
