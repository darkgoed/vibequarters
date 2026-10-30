# Segurança e privacidade — princípios

O VibeQuarters pretende conectar agentes de IA a dispositivos reais. Por isso, a segurança é parte da funcionalidade, não um complemento posterior.

## Modelo proposto

- **Código público ≠ backend público:** este repositório contém documentação, não credenciais ou serviços internos.
- **Confiança explícita:** cada computador exige pareamento por device code e consentimento para seus escopos.
- **Menor privilégio:** o serviço intermediário deve rodar sem root e acessar somente diretórios autorizados; nenhuma API aberta de shell administrativo.
- **Execução controlada:** autenticação do dispositivo, autorização por usuário e escopo, timeout, limite de saída, encerramento seguro, trilha de auditoria e confirmação de operações sensíveis/destrutivas.
- **Não confiar em conteúdo externo:** resultados de ferramentas, arquivos, nomes de agentes e mensagens podem conter instruções maliciosas. Nenhum deles concede novas permissões.
- **Tokens:** duração curta, rotação/revogação, armazenamento adequado; nunca registrar segredos em logs.
- **Conta web:** e-mail e senha com hash resistente, rate limiting, proteção de sessão, recuperação segura e monitoramento; MFA não será requisito obrigatório do MVP.
- **Cotas futuras:** contagem server-side resistente a concorrência, relatórios transparentes, prevenção de abuso e bloqueio de uso acima do permitido.
- **Incidentes:** rollback e revogação de dispositivos precisam ser possíveis sem derrubar projetos de terceiros.

## O que NÃO está disponível hoje

Não há cliente remoto público instalado por `npx`, nem conexão pública de comando do VibeQuarters para qualquer pessoa. Documentação de uma capacidade não representa um certificado de que já funciona.

## Reportar vulnerabilidades

Antes de publicar detalhes exploráveis, entre em contato privadamente com o mantenedor pelo perfil do GitHub. Não inclua tokens, credenciais, logs sensíveis ou dados de terceiros em issues públicas.
