# Ambiente Kong API Gateway

Ambiente de execucao do Kong API Gateway usando ferramenta docker-compose

## Ferramentas necessarias
* docker
* docker-compose
* editor *.yaml


## Ferramentas que serao provisionadas usando o docker-compose
* Grafana
* Prometheus
* Prometheus Node Exporter

### Arquivos de configuracao prometheus

Na pasta [prom-conf](compose/prom-conf) contem os arquivos necessarios para configuracao do prometheus, inclusive a configuracao de _scraping_ das metricas do Kong API Gateway


## Rodando

Na pasta raiz do projeto voce pode executar

```shell
docker-compose -f compose/kong_compose.yml up -d
```
