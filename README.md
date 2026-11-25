API Pets – Performance Testing

Objetivo

Projeto de testes de performance utilizando Apache JMeter para avaliar o comportamento da API Pets.

Cenários implementados

1. Modelo Fechado (Closed Workload)

Thread Group: bzm - Concurrency Thread Group

Concorrência: 50 usuários

Ramp-up: 20 segundos

Duração: 50 segundos

2. Modelo Aberto (Open Workload)

Thread Group: bzm - Arrivals Thread Group

Taxa de chegada: 1 usuário/segundo

Duração: 50 segundos

Iterações: 1 por usuário

Endpoints testados

POST /login

GET /status

POST /pets

GET /pets

Ferramentas

Apache JMeter 5.6.3

JMeter Plugins

Métricas avaliadas

Average Response Time

Median

P90 / P95 / P99

Throughput

Error Percentage

Estrutura

test-plans/: planos de teste JMeter.

results/: resultados das execuções.
