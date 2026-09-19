# Data On-Prem to Cloud

Pipeline de engenharia de dados que simula um cenário real de migração: extração de dados de um banco relacional on-premise (SQL Server), validação de qualidade e disponibilização em uma arquitetura moderna de dados na nuvem (AWS).

## Contexto e Motivação

Este projeto formaliza, como pipeline de engenharia, um processo que hoje muitas empresas ainda fazem manualmente: extrair dados de sistemas legados on-premise, garantir sua conformidade e qualidade, e disponibilizá-los em uma plataforma de dados moderna para consumo analítico.

## Arquitetura

> Diagrama detalhado em construção — ver `docs/architecture-decisions/`

- **Origem:** SQL Server 2022 (on-premise, simulado localmente)
- **Camada de extração:** scripts Python
- **Camada RAW/CURATED (local):** MinIO (simula S3) + PostgreSQL (simula Data Warehouse)
- **Validação de qualidade:** regras automatizadas de conformidade de dados
- **Camada cloud (AWS):** S3 + Glue/Athena, provisionado via Infraestrutura como Código

## Status do Projeto

🚧 Em desenvolvimento — projeto de estudo e portfólio em construção.

## Decisões de Arquitetura

Decisões técnicas relevantes (e seus trade-offs) estão documentadas individualmente em [`docs/architecture-decisions/`](./docs/architecture-decisions/).

## Stack

Python · SQL Server · Docker · PostgreSQL · MinIO · AWS (S3, Glue, Athena) · Terraform

## Autora

Roseane Molina — em transição de carreira para Arquitetura de Dados, com background em Ciências Contábeis e experiência em conformidade e migração de dados corporativos.
