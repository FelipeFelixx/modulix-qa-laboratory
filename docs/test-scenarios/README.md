# Test Scenarios

Cenários de teste do sistema sob teste.

---

## Objetivo

Documentar os cenários de teste derivados dos requisitos e critérios de
aceite do Modulix QA Laboratory, mantendo rastreabilidade entre requisito,
critério de aceite e execução.

---

## RF-001 — Health Check da API

### CEN-001 — Consultar health check com a API disponível

**Tipo:** Positivo

**Objetivo:** Verificar se o endpoint de health check está disponível e
retorna as informações esperadas sobre o serviço.

**Critérios de aceite relacionados:**

- CA-001 — HTTP `200 OK`.
- CA-002 — Resposta em JSON.
- CA-003 — Campo `status` com valor `ok`.
- CA-004 — Campo `service` com valor
  `modulix-qa-laboratory-backend`.

**Endpoint:**

`GET /health`

**Status do cenário:** IMPLEMENTADO E EXECUTADO

---

### CEN-002 — Consultar rota inexistente

**Tipo:** Negativo

**Objetivo:** Verificar se a API rejeita uma requisição para uma rota que não
está definida.

**Critério de aceite relacionado:**

- CA-005 — Uma rota inexistente deve retornar HTTP `404 Not Found`.

**Endpoint utilizado na execução:**

`GET /rota-inexistente`

**Status do cenário:** IMPLEMENTADO E EXECUTADO

---

## Rastreabilidade

| Cenário | Requisito | Critérios de aceite | Execução |
|---|---|---|---|
| CEN-001 | RF-001 | CA-001, CA-002, CA-003, CA-004 | Executada |
| CEN-002 | RF-001 | CA-005 | Executada |

---

## Observação

Os cenários acima foram derivados exclusivamente do comportamento atualmente
implementado e das execuções realizadas no ambiente local.

Novos cenários serão adicionados conforme novos requisitos e funcionalidades
forem implementados.

---

## Estado deste documento

**IMPLEMENTADO**

Os primeiros cenários de teste do RF-001 foram documentados e possuem
execuções reais correspondentes.
