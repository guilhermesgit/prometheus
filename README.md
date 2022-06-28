# prometheus
Monitorando containers utilizando o prometheus:

1)Docker compose possui 3 containers:

Grafana - Para a utilização de dashboard
CadAdivisor - monitorar os containers
Prometheus - para utilização de métricas do cadadivisor

###
Para monitorar os containers é necessário utilizar o datasource do prometheus:
- Única configuração necessária: nomedoserviço:porta

##
Dentro do prometheus é necessário observar se os targets estão com status UP porque são eles os responsáveis
para nos informar as métricas .

