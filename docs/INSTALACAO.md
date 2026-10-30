# Instalação e pareamento — planejamento

> **Ainda indisponível.** Este documento descreve a experiência futura. Não há download, pacote npm verificado nem cadastro aberto hoje.

## Por que npx?

`npx` (também disponível via `npm exec`) executa uma ferramenta publicada como pacote npm. O GitHub documentará a instalação; o código privado do servidor não precisará ficar no GitHub para que alguém utilize o produto.

## Fluxo projetado

1. O usuário instala uma versão de Node.js suportada (a versão mínima será publicada após os testes).
2. Abre terminal **no próprio computador** e confere o pacote oficial e sua assinatura.
3. Executa o instalador oficial. **Comando ilustrativo e ainda não operacional:** `npx vibequarters connect`.
4. Recebe um código temporário e um endereço HTTPS de verificação.
5. Faz login no portal, confere dispositivo e permissões solicitadas e aprova o pareamento.
6. O cliente guarda credenciais de forma segura, inicia conexão de saída e apresenta o dispositivo no escritório.
7. O usuário pode consultar, acompanhar, desconectar e revogar qualquer dispositivo.

O pareamento será baseado no **OAuth 2.0 Device Authorization Grant (RFC 8628)**, com intervalo de consulta, expiração e bloqueio de solicitações abusivas. Não se trata de MFA obrigatório; o login web inicial será por e-mail e senha com segurança reforçada.

## Primeiro teste para disponibilização

Antes de abrir a instalação para terceiros, verificar em uma máquina de teste limpa: integridade do pacote, atualização/desinstalação, device code válido e expirado, revogação, execução autorizada de `uptime` com retorno verificável, resistência a comandos perigosos, rollback, Windows/Linux/macOS suportados **somente quando efetivamente testados** e ausência de vazamento de segredo.

## Evite instalações falsas

Até o anúncio oficial:
- **não execute** o comando ilustrativo;
- não confie em pacotes homônimos ou domínios semelhantes;
- não forneça tokens, senhas ou acesso SSH a sites que afirmem ser o VibeQuarters.

Referências: [npm npx](https://docs.npmjs.com/cli/v11/commands/npx/) e [RFC 8628](https://www.rfc-editor.org/rfc/rfc8628).
