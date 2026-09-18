# Modulix QA Laboratory

**Manual QA & API Testing Laboratory**

Projeto acadêmico e de portfólio para estudo prático de Quality Assurance,
com foco em testes manuais, testes de API, validação de dados e, futuramente,
automação.

> **Status da V1:** estrutura inicial do laboratório. Resultados de testes,
> bugs e evidências somente serão marcados como executados após execução real.

## Objetivos

- Praticar QA Manual de forma estruturada.
- Criar documentação de requisitos e critérios de aceite.
- Elaborar cenários e casos de teste.
- Executar testes funcionais, exploratórios, smoke e regressão.
- Documentar defeitos e evidências.
- Praticar API Testing com Postman.
- Validar dados com SQL.
- Preparar a base para Playwright + TypeScript e CI/CD.

## Estado atual

### IMPLEMENTADO
- Estrutura inicial do repositório.
- Política inicial de segurança.
- Templates de documentação.
- Estrutura reservada para frontend, backend, banco, API e evidências.

### PARCIALMENTE IMPLEMENTADO
- Nenhuma funcionalidade de aplicação ou API é considerada implementada nesta etapa.

### PLANEJADO
- Aplicação web de laboratório.
- Backend REST.
- PostgreSQL.
- Collection Postman.
- Massa de dados fictícia.
- Execução documentada dos testes.
- Automação com Playwright + TypeScript.
- CI/CD com GitHub Actions.

## Segurança

Este repositório foi planejado para ser público.

**Nunca commite:**
- `.env` ou arquivos equivalentes com valores reais;
- senhas;
- tokens;
- API keys;
- chaves privadas;
- certificados privados;
- cookies/sessões;
- credenciais de serviços;
- dados pessoais reais.

Use `.env.example` apenas como modelo, sem segredos.

Consulte [SECURITY.md](SECURITY.md).

## Estrutura

```text
frontend/       Aplicação web sob teste
backend/        API/backend sob teste
database/       Schema, seed e SQL de validação
api/             Materiais de API/Postman
qa/              Artefatos de QA
docs/            Documentação complementar
evidence/        Evidências reais após execução
reports/         Relatórios reais após execução
```

## Regra de evidência

Nenhum teste será declarado PASS/FAIL sem execução real.
Nenhum bug será declarado encontrado sem evidência ou registro correspondente.

## Licença

Projeto acadêmico e de portfólio da Modulix.
