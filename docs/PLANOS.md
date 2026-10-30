# Modelo freemium — hipótese comercial

> **Planejamento para depois do MVP.** Não há preços anunciados, pagamentos ativos ou limite final estabelecido.

## Proposta inicial

| Acesso futuro | Hipótese de produto | Ainda não definido |
| --- | --- | --- |
| Free | Escritório e chamadas remotas básicas com cota | Quantidade, duração, limites por dispositivo |
| Pro | Cotas maiores, mais concorrência, histórico e suporte | Valor, capacidade, suporte |
| Lifetime (em avaliação) | Licença de software por pagamento único | Condições, uso justo, infraestrutura e suporte |

### Janelas de uso a testar

Podemos combinar: limite em **janela de 5 horas**, limite **semanal** e limite **mensal**, reiniciados conforme o relógio do servidor. Uma chamada pode consumir cota e ainda ser recusada por motivo de segurança.

Não escolher quantidades arbitrárias: primeiro medir no beta o custo da conexão, volume, CPU, tempo, armazenamento, abusos e suporte. Definir quando uma chamada falha ou é cancelada se deve consumir ou devolver crédito. Exibir no painel uso restante e horário real de reset.

### Por que não prometer ilimitado vitalício?

Mesmo quando o software é licenciado uma vez, operar um serviço remoto tem custo recorrente. Uma licença Lifetime, se existir, não deverá garantir processamento ilimitado de infraestrutura por tempo indefinido. O contrato precisará definir uso justo, duração de suporte, atualizações e continuidade.

### Distribuição e proteção do código

O GitHub público hospeda explicação e instruções verificadas. O cliente de dispositivo poderá ser distribuído como pacote npm quando estiver pronto, mas o backend e o núcleo de controle permanecem hospedados/fechados. Código distribuído não é impossível de analisar ou replicar.

Nenhuma cobrança será iniciada antes da segurança, do isolamento entre clientes e da contabilidade auditável passarem nos testes.
