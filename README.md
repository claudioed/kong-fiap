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

Na pasta [prom-conf](compose/prom-conf) contem os arquivos necessarios para configuracao do prometheus, 
inclusive a configuracao de _scraping_ das metricas do Kong API Gateway


## Rodando

Na pasta raiz do projeto voce pode executar

```shell
docker-compose -f compose/kong_compose.yml up -d
```

Kong API Gateway
Papel: Atua como uma camada entre os clientes e os serviços de backend. É responsável por receber as requisições de APIs, aplicar políticas de segurança, gerenciar o tráfego, rotear pedidos e otimizar as respostas.
Característica vital: Extensibilidade através de plugins, que permite customizar e estender suas funcionalidades para autenticação, segurança, controle de tráfego, entre outros.
Prometheus
Papel: Sistema de monitoramento que coleta métricas de diversas fontes, armazenando-as de forma eficiente e oferecendo uma poderosa linguagem de consulta para análise de desempenho.
Característica vital: Modelo de dados multidimensional com suporte a séries temporais, o que permite uma análise detalhada e em tempo real do comportamento e desempenho das aplicações.
Grafana
Papel: Ferramenta de visualização de dados que permite criar dashboards dinâmicos para visualizar métricas complexas de diversas fontes, incluindo Prometheus.
Característica vital: Capacidade de integrar e visualizar dados de diversas fontes simultaneamente, proporcionando uma visão abrangente e detalhada do desempenho da infraestrutura e das aplicações.
Konga
Papel: Painel de administração para o Kong API Gateway, facilitando a gestão e configuração de suas funcionalidades de forma visual e intuitiva.
Característica vital: Interface amigável ao usuário, que simplifica a administração do Kong API Gateway, tornando acessível até para aqueles com menos experiência técnica em linha de comando.
Cada uma dessas ferramentas desempenha um papel crítico em garantir que a gestão, o monitoramento e a visualização das APIs sejam eficientes, seguras e escaláveis.
