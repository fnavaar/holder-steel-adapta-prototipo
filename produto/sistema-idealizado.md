# Sistema idealizado

Fonte operacional única por obra, do fechamento à entrega de material aceito, com números e condições financeiras ligados desde a origem. Gerar primeiro valor utilizável, não apenas dashboards sem dados.

Navegação candidata: visão de obras → obra escolhida → resumo, documentos, pendências e Lista Master. Revisões, suprimentos, compras, cargas e financeiro aparecem conforme capacidade de fase construída/aceita; futuro é planejado, nunca botão falso.

Fluxo: Comercial informa obra/condições; Planejamento organiza handoffs/metas; Projetos valida revisão/identidade; Suprimentos compara e registra decisão/OC; Obras confirma físico; Financeiro classifica/reconcilia; Gestão consulta origem/cobertura. Retornos e correções mantêm histórico.

## 6. Fases e módulos recriados

Rótulos abaixo são **IDs de proposta**, não UUIDs do portal. Fases futuras têm arco/resultados; somente F1 recebe detalhamento agora. Prazo de quatro meses preservado; nenhum calendário novo inventado.

| Fase | Módulos propostos | Resultado da fase |
|---|---|---|
| F1 — Organizar a obra e a informação | F1-M01 Obra e documentos; M02 Pendências; M03 Lista Master; M04 Medição; M05 Saldo assistido | Uma obra consultável com passagem entre áreas, lista vigente e limites explícitos; baseline/modelo financeiro iniciados |
| F2 — Preparar projeto e compra | F2-M01 Revisões e peso; M02 orçamento/meta e marcos; M03 propostas e decisão de fornecimento | Cotar/decidir com escopo, referência, meta e condições rastreáveis |
| F3 — Acompanhar atendimento e números da obra | F3-M01 solicitação/OC; M02 cargas/aceite/divergências; M03 eventos financeiros/saldo contratual; M04 visão integrada da obra | Material aceito e números reconciliáveis, sem confundir estoque, faturamento ou caixa |
| F4 — Operar com apoio de IA | F4-M01 resumo de pendências/material; M02 preparação de consolidação financeira | Loops sobre registros homologados; revisão humana; metas/acessos a pactuar |
| F5 — Validar o conjunto | F5-M01 jornada completa; M02 resultado/adoção e próxima evolução | Demonstrar sistemas e loops efetivamente ativados, comparar amostras e registrar limitações |

**Atenção de capacidade:** antecipar capacidades da F4/F5 antiga para F3 aumenta a concentração nessa fase. Não há prova de impossibilidade nem capacidade que permita garantir encaixe. Sequenciar por incrementos e validar recorte antes da migração; não reduzir promessa tacitamente.

### Mapeamento das funcionalidades de origem

| Escopo base | Novo lugar | Preservação |
|---|---|---|
| 4.1 cadastro/kick-off | F1-M01 | condições e documentos desde origem |
| 4.2 checklist | F1-M02 | prontidão explícita sem liberar compra implicitamente |
| 4.3 meta | F2-M02 | percentual validado, orçamento origem e regras humanas |
| 4.4 revisão/peso | F1-M03 + F2-M01 | referência primeiro; comparação e decisão técnica depois |
| 4.5 fornecedores | F2-M03 | escolha humana, não ranking autônomo |
| 4.6 validação contratação | F2-M03 + F3-M01 | valor/fornecedor/faturamento contra regra aprovada |
| 4.7 compras/provisões | F3-M01 + F3-M03 | pedido antes de NF; estados distintos |
| 4.8 NF/despesas | F3-M03 | documentos/eventos e pendências financeiros |
| 4.9 expedição/recebimento | F3-M02 | romaneio e conferência física separados |
| 4.10 RNC/divergência | F3-M02 | responsável, prova, reposição e impacto humano |
| 4.11 gerencial | F3-M04 + F5-M02 | visão implantada antes da validação final |
