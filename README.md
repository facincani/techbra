# Projeto Final End-to-End

> Projeto em grupo, tema livre. 

## Descrição

Construa um fluxo completo de negócio (ex.: pedidos, assinaturas, billing, logística) com arquitetura hexagonal, BFF, mensageria (Kafka/Rabbit), resiliência, cache, observabilidade e deploy em Kubernetes via Helm. Infra de dev provisionada por Terraform. Documentação viva (C4 + ADRs) e automação de CI/CD.

## Entregáveis

-  Repositório com código, README de execução, /docs (C4 + ADRs), docker-compose, charts Helm, Terraform (dev).
-  Dashboards (métricas/tracing) e runbook curto de incidentes.
-  PR final integrando tudo.

## Critérios de avaliação (com pesos)

-  20% Arquitetura & Domínio: portas/adaptadores, linguagem ubíqua, testes de use case.
-  20% Mensageria & Orquestração: tópicos/filas, idempotência, Saga (coreografia ou orquestração) e/ou CQRS.
-  15% BFF & Contrato: view models centrados no cliente, fallback sem vazar domínio.
-  10% Cache & Desempenho: L1/L2, invalidação por evento, métricas p95/p99.
-  10% Resiliência: timeouts, retry com jitter, circuit breaker, bulkhead/rate limit.
-  10% Kubernetes & Helm: probes, rollout, HPA, NetworkPolicy.
-  10% IaC & CI/CD: Terraform (state remoto), pipeline validate > plan > apply.
-  5% FinOps & Governança: tags, budget/alertas, quotas ou KEDA.
