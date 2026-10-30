# VibeQuarters

**Seu escritório de agentes de IA — em pixel art, conectado ao trabalho real.**

> 🚧 **Pré-lançamento / projeto em validação privada.** Este repositório contém somente documentação pública. **O instalador ainda NÃO foi publicado**. Não existe uma versão pronta para instalar ou contratar aqui.

O VibeQuarters está sendo desenvolvido para pessoas que usam agentes de IA para programar (*vibe coding*). A ideia é acompanhar o que os agentes estão fazendo em um escritório pixelado e, com sua autorização, consultar e operar a própria máquina por um assistente.

## O que estamos construindo

- **Escritório pixelado:** salas, personagens e estados ligados a agentes reais, não apenas animações fictícias.
- **Integração com Hermes:** visualizar sessões, projetos, atividades e estados verificáveis.
- **Conexão MCP / Code Mode:** acessar arquivos permitidos e executar comandos autorizados no seu dispositivo por um agente local seguro.
- **Pareamento por código:** conectar uma máquina iniciando no terminal e aprovando um código no navegador (OAuth Device Authorization Grant).
- **Conta e dispositivos:** autenticação, revogação, logs e controles de segurança.

A execução remota **não** significa expor um shell root na internet. O usuário controla quais dispositivos conecta e quais ações autoriza.

## Instalação

**Ainda não disponível.** O fluxo planejado terá esta forma:

1. Instalar o Node.js em versão suportada e abrir um terminal.
2. Executar o instalador oficial publicado por nós no **npm**, usando `npx`.
3. Acessar um endereço de verificação, entrar na conta e aprovar o *device code* exibido no terminal.
4. Visualizar seus agentes e sua máquina no escritório.

**Exemplo de comando desejado para o futuro (não execute agora):**

```bash
npx vibequarters connect
```

Esse nome de pacote e esse comando **não estão validados nem publicados**. Antes do lançamento, divulgaremos aqui o pacote npm verificado, o domínio oficial e os requisitos reais. Não execute pacotes com nomes semelhantes encontrados por conta própria.

Veja [Instalação e pareamento — planejamento](docs/INSTALACAO.md).

## Estado do projeto

| Etapa | Situação |
| --- | --- |
| Produto e marca VibeQuarters | Definidos provisoriamente |
| MVP pessoal com agentes Hermes reais | Em desenvolvimento privado |
| Conexão MCP/Code Mode ponta a ponta | Pendente de validação real |
| Instalador npm/npx assinado e auditado | **Não publicado** |
| Cadastro público, cotas e planos | Fase futura |
| Lançamento aberto | **Não anunciado** |

Nosso primeiro marco é fazer o MVP funcionar de ponta a ponta para o usuário inicial. **Não aceitamos pagamentos e não oferecemos instalações públicas nesta fase.**

## Como funcionará o freemium

A intenção é ter acesso gratuito com cotas de chamadas remotas e opções pagas para uso maior. Estudamos janelas de cinco horas, semanais e mensais, mas **preços e limites não foram definidos**. A interface pixelada e as ações remotas poderão ter regras de consumo diferentes.

Leia [Modelo freemium em estudo](docs/PLANOS.md) e [Roadmap](docs/ROADMAP.md).

## Por que só documentação pública?

A experiência será disponibilizada pelo site e por um pequeno cliente de dispositivo quando estiver pronto. O backend hospedado, a infraestrutura de autenticação, os controles de acesso e a lógica comercial **não serão publicados neste repositório**. Instalar o cliente não implica receber o código-fonte do serviço.

Este repositório **não é o repositório de desenvolvimento do aplicativo**, não contém tokens, código interno, servidores ou arquivos privados e não concede licença para redistribuir um software inexistente.

## Acompanhe

Você pode marcar este repositório com **Star** ou **Watch** para acompanhar os anúncios. O nome e os futuros domínios oficiais só serão confirmados após a verificação de marca e disponibilidade.

Documentação: [Segurança](docs/SEGURANCA.md) · [Roadmap](docs/ROADMAP.md) · [Instalação planejada](docs/INSTALACAO.md)

---

*VibeQuarters é um nome de trabalho. Não há oferta pública de software ou planos neste momento.*
