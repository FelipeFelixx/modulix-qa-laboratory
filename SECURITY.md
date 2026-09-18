# Security Policy

## Objetivo

O Modulix QA Laboratory é um projeto público de estudo e portfólio.
A segurança do repositório é tratada como requisito desde a primeira versão.

## Dados permitidos

Use exclusivamente:
- dados fictícios;
- credenciais de teste sem valor real;
- chaves/segredos locais não versionados;
- exemplos anonimizados.

## Nunca publicar

- senhas reais;
- tokens;
- API keys;
- JWT secrets;
- chaves privadas;
- certificados privados;
- cookies de autenticação;
- arquivos `.env` com valores;
- dados pessoais reais;
- credenciais de banco ou serviços externos.

## Tratamento de segredo publicado

Se um segredo real for publicado acidentalmente:
1. interrompa o uso da credencial;
2. revogue ou rotacione a credencial;
3. remova o segredo do histórico quando necessário;
4. verifique os logs e acessos;
5. registre a ocorrência.

Remover um segredo apenas do arquivo atual não torna uma credencial previamente exposta segura.

## Vulnerabilidades

Este laboratório pode futuramente conter cenários deliberadamente vulneráveis
para fins educacionais. Esses cenários deverão ser claramente documentados e
não deverão utilizar sistemas, contas ou dados reais.

## Reporte

Para vulnerabilidades do próprio repositório, registre uma issue sem incluir
segredos ou informações sensíveis. Para uma vulnerabilidade que contenha
informação sensível, não publique a informação diretamente em uma issue pública.
