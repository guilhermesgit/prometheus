
# Instalando o prometheus utilizando docker

Arquivo de configuração do docker compose para instalar do prometheus,grafana e cadvisor.

Monitorando containers utilizando o prometheus:

1)Docker compose possui 3 containers:

Grafana - Para a utilização de dashboard CadAdivisor - monitorar os containers Prometheus - para utilização de métricas do cadadivisor

Para monitorar os containers é necessário utilizar o datasource do prometheus:

Única configuração necessária: nomedoserviço:porta
Dentro do prometheus é necessário observar se os targets estão com status UP porque são eles os responsáveis para nos informar as métricas .
## Instalação

Para instalar os 3 containers é necessário rodar o docker-compose
```bash
  docker-compose up -d dentro do diretório do yml file.
  
  Depois:
  
  docker-compose ps e, se os containers estiverem run, acessar os containers
  
  prometheus: ipaddress:9090
  cadvisor:   ipaddress:8888
```


## Referência

 - [Referência prometheus](https://prometheus.io/docs/guides/cadvisor/)


## Autor

- [@guilhermesgit](https://www.linkedin.com/in/guilherme-s-69ab8a146/)


## Documentação

[Prometheus docker](https://prometheus.io/docs/prometheus/latest/installation/)

[Cadvisor docker](https://github.com/google/cadvisor)


