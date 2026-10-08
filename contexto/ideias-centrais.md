# Ideias centrais do projeto Holder Steel

Este é o mapa principal do contexto. Ele organiza a informação útil do Drive por problema e decisão de produto, em vez de reproduzir pastas, transcrições, planilhas, desenhos ou gravações. A estrutura detalhada e legível por máquina está em `ideias-centrais.json`; a cobertura das fontes está em `cobertura-fontes-drive.md`.

## Como ler

- **Confirmado**: observado nas fontes ou validado na autoria do projeto.
- **Proposto**: direção de produto ainda sujeita a desenho e confirmação.
- **Pendente**: pergunta que muda regra, dado, integração, permissão ou aceite.
- **Fora do ciclo**: ideia registrada para não se perder, sem autorização de implementação.
- Arquivo presente, proposta documentada e publicação no Git não equivalem a autorização para construir ou ativar.

## IC-01 — Escalar obras com informação confiável

**Informação central:** a Holder Steel quer ampliar a capacidade de executar obras simultâneas sem perder qualidade, prazo, segurança e atendimento. O problema transversal é a fragmentação da informação entre pessoas, planilhas, mensagens, pastas e ERP, que torna lenta e sujeita a erro até uma pergunta básica sobre uma obra.

**Valor esperado:** uma visão integrada por obra, com origem, atualização e cobertura visíveis, reduzindo procura, redigitação, conferências repetidas e dependência de pessoas-chave. Não há percentual de ganho prometido sem baseline real.

**Fronteira atual:** o ciclo prioriza o caminho do fechamento do contrato à entrega e aceitação do material, com o financeiro da obra conectado. CRM, RH, marketing, cálculo estrutural por IA e substituição integral do ERP permanecem fora do ciclo.

## IC-02 — A obra é o eixo comum entre áreas

**Informação central:** Comercial e Orçamento iniciam a passagem com escopo, proposta, condições, datas e documentos. Planejamento transforma isso em kick-off, marcos e pendências por área. Hoje o handoff pode ocorrer antes de o contrato estar assinado e usa e-mail, WhatsApp, planilhas e pastas.

**Ideia de produto:** uma identidade estável de obra reúne escopos, revisões, documentos, condições, participantes, marcos e pendências. Rascunho, registro validado, assinatura e liberação são estados distintos. Pendência sem dono continua visível; conclusão exige evidência e pode ser reaberta com motivo.

**Pendente:** obra piloto, usuários, documentos autorizados, alçadas e o projeto Skip/SkipCloud que deve ser reutilizado.

## IC-03 — Lista Master e famílias documentais

**Informação central:** não existe um único formato de lista. As fontes mostram resumos de peso, listas de telhas, painéis e arremates, tabelas de reações, planilhas de suprimentos e desenhos. Elas variam em identidade, revisão, marca, descrição, unidade, quantidade, dimensões, material, acabamento, peso e fórmulas.

**Ideia de produto:** preservar o original e normalizar por família documental. A carga passa por prévia, validação e confirmação. Código, marca, unidade, quantidade ou peso ausentes não podem ser inventados. Uma revisão nova não apaga a anterior; a referência vigente é escolhida por autoridade técnica e pode ser recuperada.

**Exceção crítica:** resumo de peso não é lista de peças. Referência documental não libera fabricação e não altera saldo físico por si.

## IC-04 — Projeto, revisão e comparação de peso

**Informação central:** Projetos recebe o escopo e documentação, coordena cálculo/detalhamento com parceiros e compara o peso orçado com o calculado. As fontes mostram ciclos de retrabalho quando o cálculo excede a referência comercial, navegação entre Excel, CAD/BIM, e-mail e pastas, e risco de usar arquivo desatualizado.

**Ideia de produto:** vincular cada documento, Lista Master e comparação à obra, escopo e revisão. Mostrar diferenças apenas quando as bases forem completas e comparáveis. Readequação técnica, tolerância, aprovação de engenharia de valor e liberação continuam humanas.

**Pendente:** regra de tolerância de peso, software/fonte oficial de projeto, padrão de nomenclatura e autoridade que ativa uma revisão.

## IC-05 — Suprimentos decide com rastreabilidade

**Informação central:** materiais são agrupados e reorganizados manualmente por família e fornecedor. Há cotação, equalização de preço, prazo e solução, além de combinações distintas de fornecimento, industrialização e faturamento. Três propostas e redução aproximada de 10% aparecem como práticas observadas, não como políticas aprovadas.

**Ideia de produto:** gerar uma meta de suprimentos a partir de fonte identificada, comparar propostas sobre o mesmo escopo e registrar fornecedor, razão, autor, data, exceção e impacto. O sistema apoia a decisão; não escolhe fornecedor nem aprova contratação.

**Pendente:** alçadas, número mínimo de propostas, regras de meta/desconto e tratamento formal de engenharia de valor.

## IC-06 — Compra e ordem de compra têm estados reais

**Informação central:** solicitações chegam por e-mail ou WhatsApp e são redigitadas no SIGO. Cadastro de obra, endereço, material, condição de faturamento, vencimento, anexos e não conformidade podem exigir tratamento manual. Emissão, envio, confirmação do fornecedor, provisão, NF e pagamento não são o mesmo evento.

**Ideia de produto:** vincular solicitação, proposta, decisão, OC, itens, revisão, condição de faturamento, anexos e estados. Repetição não duplica evento. Se a emissão oficial permanecer no ERP, o produto registra número, estado e evidência sem emitir duas vezes.

**Pendente:** alçadas de OC, regras de vencimento, fonte oficial dos cadastros e possibilidade real de integração com o SIGO.

## IC-07 — Expedição, recebimento e saldo material

**Informação central:** romaneios e dados de carga circulam por canais dispersos. Obras confere fisicamente, muitas vezes em papel, e comunica faltas ou danos. Um romaneio descreve uma carga; não comprova que todo o escopo chegou. A ausência de Lista Master integrada aos romaneios dificulta saber se a montagem pode prosseguir.

**Ideia de produto:** separar requerido, expedido, recebido, aceito, divergente, recusado, reposto e devolvido. O saldo material atendido é `requerido - aceito`; não é estoque disponível nem prova automática de prontidão para montagem. Aceite parcial mantém o restante pendente. Reposição não pode duplicar atendimento.

**Pendente:** responsável por aceite, padrão mínimo de romaneio, contingência de campo e tratamento oficial de RNC/reposição.

## IC-08 — Financeiro da obra é uma cadeia de eventos reconciliável

**Informação central:** contrato, aditivo, OC, provisão, faturamento próprio, faturamento direto, NF, cancelamento e pagamento vivem em fontes e momentos diferentes. NFs podem chegar por e-mail e ser lançadas manualmente. O status operacional do ERP nem sempre representa liquidação bancária.

**Ideia de produto:** manter eventos separados, com documento, categoria, origem, data, cancelamento e vínculo à obra. O saldo contratual a faturar parte do contrato vigente e aditivos aprovados, menos faturamentos homologados que o consomem. A fórmula, as categorias e o faturamento direto precisam de homologação financeira e reconciliação independente.

**Exceções críticas:** provisão não é pagamento; NF não é liquidação; faturamento direto não pode ser contado duas vezes; saldo a faturar não é lucro; cobertura parcial não vira saldo oficial.

## IC-09 — Gestão mede cobertura antes de afirmar resultado

**Informação central:** a empresa quer acompanhar orçamento, compromissos, material, cronograma, custos e resultado por obra. Hoje faltam métricas e o levantamento é manual. Métricas extraídas de vídeos descrevem a demonstração gravada e não são baseline operacional confiável por si.

**Ideia de produto:** todo indicador mostra conceito, fonte, atualização, cobertura e caminho até o documento ou cálculo. A coleta inicial prioriza até três métricas: minutos para consolidar saldo físico, minutos para consolidar saldo contratual e proporção de handoffs devolvidos/corrigidos. Amostra, janela, complexidade, dono e método precisam ser definidos antes de comparar antes/depois.

## IC-10 — Segurança, histórico e recuperação são parte da função

**Informação central:** dados comerciais, financeiros e documentos da obra exigem acesso por perfil e por obra. O histórico não pode expor conteúdo restrito. Importação, edição concorrente, repetição e falha parcial não podem apagar ou sobrescrever silenciosamente o estado válido.

**Ideia de produto:** autorização no servidor, isolamento entre obras, documentos privados, auditoria, idempotência, versionamento e recuperação são critérios de aceite, não detalhes posteriores. Dados ausentes permanecem ausentes; `null` não significa zero, autorizado ou verificado.

## IC-11 — Decisões e exceções permanecem humanas

**Informação central:** regras que mudam contrato, projeto, fornecedor, compra, aceite físico, fórmula financeira, resultado ou envio externo dependem de pessoas nomeadas. Terceiros podem continuar nos canais atuais; a resposta consolidada pelo Champion é a entrada oficial do projeto.

**Ideia de produto:** cada pendência tem dono, marco e efeito no domínio afetado. Falta de informação bloqueia somente o cálculo ou ação dependente, sem congelar todo o sistema. O produto mantém estados finais válidos e sempre oferece correção, reabertura ou recuperação rastreável.

## IC-12 — Assistente e loops controlados

**Informação central:** há oportunidade de o assistente preparar resumos de material e consolidações financeiras usando fontes já homologadas. Esses loops dependem dos sistemas das fases anteriores, de acesso confirmado, meta mensurável, cadência e validador humano.

**Ideia de produto:** o assistente prepara, explica e aponta evidências. Ele não envia cobrança, cria compra, aprova projeto, aceita material, lança despesa, muda fórmula nem paga. Fonte indisponível pausa o ciclo. Nenhum loop está ativo por este pacote.

## Ideias registradas para depois

As fontes também citam CRM e orçamentos, horas extras, diário de obra, vistorias, produtividade, segurança, pessoas, conteúdo de marketing, BIM móvel e QR code. Elas permanecem em `produto/ideias-para-depois.md`, separadas do ciclo vigente para não desaparecerem nem ampliarem o escopo por acidente.

## Regra de atualização

Toda nova fonte do Drive deve alterar pelo menos um destes artefatos:

1. `ideias-centrais.md` e `ideias-centrais.json`, quando mudar o significado;
2. `cobertura-fontes-drive.md`, quando mudar a cobertura ou surgir nova família;
3. `fontes.json`, quando mudar a proveniência;
4. módulo, função, critério ou decisão correspondente, quando a mudança estiver autorizada.

