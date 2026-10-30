# Roadmap do VibeQuarters

Este roadmap descreve **objetivos**, não funcionalidades já entregues. A fonte de verdade do desenvolvimento é a QA privada e os testes de aceitação, não este repositório público.

## Fase 0 — MVP privado (prioridade absoluta)

- [ ] Escritório Pixel World publicado no domínio privado do proprietário, substituindo a interface anterior.
- [ ] Login por e-mail e senha protegido, sessão e recuperação de conta testadas.
- [ ] Agentes e projetos Hermes **reais**, com estados verificados; desconhecido deve continuar como `unknown`.
- [ ] Broker local com UID isolado, diretórios autorizados e auditoria.
- [ ] API MCP e Code Mode interoperáveis, com pareamento seguro e revogação.
- [ ] Teste ponta a ponta: ChatGPT/cliente compatível → dispositivo autorizado → comando benigno → stdout/exit code verdadeiros.
- [ ] QA visual e funcional, segurança, backup, deploy atômico e rollback comprovados.

**Critério de conclusão:** usar tudo em ambiente real como usuário final, sem substituir a integração por fixtures ou mock.

## Fase 1 — Instalador privado testado

- [ ] Cliente leve e documentado para o dispositivo.
- [ ] Pacote npm oficial com integridade e assinatura verificável, comando `npx` funcional.
- [ ] Fluxo completo OAuth Device Authorization Grant e desligamento/revogação.
- [ ] Matrizes de compatibilidade e instalação/desinstalação em plataformas suportadas.
- [ ] Auditoria de supply chain, dependências e atualização segura.

## Fase 2 — Beta fechado

- [ ] Isolamento por contas/dispositivos, consentimento, revogação e monitoramento.
- [ ] Medir custo real por chamada, tempo de execução, tamanho de saída e infraestrutura.
- [ ] Quotas confiáveis e UX de erro/limites.
- [ ] Abrir poucos convites após evidências de segurança e suporte.

## Fase 3 — Freemium público

- [ ] Preços e janelas de cota definidos por medição.
- [ ] Planos, billing, pagamentos, políticas de estorno e termos.
- [ ] Onboarding público, página de instalação, tutoriais e materiais para criadores.
- [ ] Monitoramento de fraudes, suporte e operação comercial.

**Não antecipar as fases comerciais em prejuízo do MVP.**
