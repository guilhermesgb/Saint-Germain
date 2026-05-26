# Premier — Atualização de Estoque

**Rodada:** 26/05/2026 12:13 UTC (terça-feira, dia útil)
**Janela buscada:** `after:2026/05/24` (Gmail) — desde a última rodada (25/05 16:14 UTC).

## 1. Resumo das atualizações aplicadas

| Processo | ID | Tipo | Mudança aplicada |
|----------|-----|------|------------------|
| SG.096/25 | 59 | A (complemento) | Append em `observacoes`: "26/05/2026: Premier enviou fechamento do processo. Saldo pendente de R$ 365,14 a ser pago (comprovante a encaminhar)." `updated_at` atualizado. |

**Nenhuma mudança de grupo** nesta rodada → não foi necessário recalcular `ordem`.

## 2. Threads inspecionadas

Foram retornadas 8 threads de FOLLOW UP Premier na busca `after:2026/05/24`:

| Numerário | Data thread | Status na thread | Já registrado? |
|-----------|-------------|------------------|----------------|
| SG.096/25 | 26/05/2026 | Fechamento (R$ 365,14 pendente) | **NÃO — aplicado nesta rodada** |
| SG.103A/26 | 25/05/2026 | Embarcada (sem novidades) | Sim (rodada anterior) |
| SG.106A/26 | 25/05/2026 | Coletada + booking aéreo | Sim (rodada anterior) |
| SG.132/26 | 25/05/2026 | Câmbio fechado USD 61.329,00 | Sim (rodada anterior) |
| SG.131/26 | 25/05/2026 | Câmbio fechado USD 5.476,50 | Sim (rodada anterior) |
| SG.130/26 | 25/05/2026 | Câmbio fechado USD 3.452,55 | Sim (rodada anterior) |
| SG.129/26 | 25/05/2026 | Câmbio fechado USD 20.380,20 | Sim (rodada anterior) |
| SG.098/26 | 25/05/2026 | Transferência + presença de carga OK | Sim (rodada anterior) |

## 3. Decisões / justificativas para casos ambíguos

- **SG.096/25 (Fechamento):** O processo já estava `conclusao='Concluído'` desde 21/05/2026 (DANFE recebida). O fechamento de hoje é evento administrativo (saldo de R$ 365,14 a pagar), não altera `prontidao` nem `conclusao`. Aplicado apenas como append em `observacoes` para histórico. **Ação para o usuário:** encaminhar comprovante de R$ 365,14 quando pago.
- **MYC GIFT (Coco) — Threads diretas com fornecedor (PI26008-SG WATCHES+JEW+SUNGLASSES+BAND e AX019B/AX019C):** 2 threads novas hoje do exportador, sem numerário SG atribuído pela Premier. Convenção observada no histórico: novos processos só são abertos quando a Premier emite um FOLLOW UP com numerário SG.xxx/26. **Sem ação no banco** — aguardar formalização.

## 4. Monitor de limbo pós-chegada (Passo 5)

Query retornou **1 processo** em limbo (chegada > 2 dias, ainda Em andamento):

| ID | Numerário | Fornecedor | Prontidão | Chegada | Dias após | Status / Ação |
|----|-----------|------------|-----------|---------|-----------|---------------|
| 57 | SG.098/26 | Yuki | `No porto` | 18/05/2026 | 8 | Sem ação — última atualização Premier em 25/05/2026 (apenas 1 dia). Container já transferido para terminal secundário, mapa liberado, presença de carga OK. Aguardando registro da importação (numerário solicitado). Status `No porto` correto. |

## 5. Pendências de cobrança

**Nenhuma** — todos os processos em limbo têm atualização Premier dentro dos últimos 5 dias.

## 6. Snapshot pós-rodada

| Grupo | Conclusão | Contagem |
|-------|-----------|----------|
| coletadas | Concluído | 65 |
| coletadas | Em andamento | 7 |
| faltam | Em andamento | 29 |
| **TOTAL** | | **101** |

## 7. Observação adicional (sem ação no banco)

- **MYC GIFT — PI26008** (26/05 11:07): Coco enviou nova Proforma Invoice de WATCHES+JEW+SUNGLASSES+BAND solicitando confirmação e arranjo do depósito. Aguardar formalização pela Premier.
- **MYC GIFT — AX019B/AX019C** (26/05 02:47): Coco solicita indicação de forwarder para embarque do AX019-B (finalizado 23/05). AX019-C pronto previsto 05/06/2026. Sem numerário SG associado ainda — aguardar Premier.

## Sources

- [SG.096/25 FOLLOW UP — Fechamento (26/05)](https://mail.google.com/mail/u/0/#inbox/19e642712958f832)
- [SG.098/26 FOLLOW UP — Transferência (25/05)](https://mail.google.com/mail/u/0/#inbox/19e5f01b342fa67b)
- [SG.103A/26 FOLLOW UP (25/05)](https://mail.google.com/mail/u/0/#inbox/19e5f65a0e5dc98e)
- [SG.106A/26 FOLLOW UP (25/05)](https://mail.google.com/mail/u/0/#inbox/19e5f51d73f8eb79)
- [SG.132/26 FOLLOW UP (25/05)](https://mail.google.com/mail/u/0/#inbox/19e5f4e49e35d45a)
- [SG.131/26 FOLLOW UP (25/05)](https://mail.google.com/mail/u/0/#inbox/19e5f4da8a908344)
- [SG.130/26 FOLLOW UP (25/05)](https://mail.google.com/mail/u/0/#inbox/19e5f4d0b496f003)
- [SG.129/26 FOLLOW UP (25/05)](https://mail.google.com/mail/u/0/#inbox/19e5f4c917cca5b7)
- [MYC PI26008 (26/05)](https://mail.google.com/mail/u/0/#inbox/19e63fae197f5ac3)
- [MYC AX019B/AX019C forwarder request (26/05)](https://mail.google.com/mail/u/0/#inbox/19e622ec0b709b30)
