# Requirements

Requisitos funcionais e critérios de aceite do sistema sob teste.

---

## RF-001 — Health Check da API

### Objetivo

Disponibilizar um endpoint que permita verificar se o backend do
Modulix QA Laboratory está operacional.

### Endpoint

GET /health

### Critérios de aceite

| ID | Critério |
|---|---|
| CA-001 | A requisição `GET /health` deve retornar HTTP `200 OK`. |
| CA-002 | A resposta deve possuir conteúdo JSON. |
| CA-003 | O campo `status` deve possuir o valor `ok`. |
| CA-004 | O campo `service` deve possuir o valor `modulix-qa-laboratory-backend`. |
| CA-005 | Uma rota inexistente deve retornar HTTP `404 Not Found`. |

### Estado da implementação

**IMPLEMENTADO**

O endpoint `GET /health` está implementado no backend.

### Validação realizada

Os seguintes comportamentos foram executados manualmente:

| Critério | Execução | Resultado observado |
|---|---|---|
| CA-001 | `GET /health` | HTTP `200 OK` |
| CA-002 | `GET /health` | `Content-Type: application/json` |
| CA-003 | `GET /health` | `status: ok` |
| CA-004 | `GET /health` | serviço identificado corretamente |
| CA-005 | `GET /rota-inexistente` | HTTP `404 Not Found` |

### Teste automatizado relacionado

O comportamento principal também possui teste automatizado em:

`backend/tests/app.test.ts`

Resultado da execução registrada:

- Test Files: 1 passed
- Tests: 1 passed

### Observação

Os resultados acima representam execuções realizadas durante o desenvolvimento
do laboratório. Novas alterações no backend deverão passar por nova execução
dos testes aplicáveis.

---

## Estado deste documento

**IMPLEMENTADO PARCIALMENTE**

O primeiro requisito foi documentado. Os demais requisitos do sistema sob teste
serão adicionados conforme novas funcionalidades forem definidas e
implementadas.
