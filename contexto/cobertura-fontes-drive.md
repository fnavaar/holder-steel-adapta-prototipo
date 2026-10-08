# Cobertura das fontes do Drive

## Resultado da auditoria

Snapshot auditado em 08/10/2026: **132 arquivos**, sem erro de leitura.

| Tipo | Quantidade | Tratamento no repo |
|---|---:|---|
| Markdown | 77 | Conteúdo útil consolidado nas ideias, decisões, módulos e critérios |
| JSON | 10 | Estado e trilha metodológica classificados; logs internos não publicados como regra de negócio |
| Excel | 11 | Estruturas e famílias documentais incorporadas; dados reais e valores não copiados |
| PDF | 22 | Tipos documentais, identidade e revisão incorporados; desenhos e documentos brutos não copiados |
| MP4 | 11 | Representados por transcrição ou análise derivada quando disponível; bruto não versionado |
| Atalho Google Docs | 1 | Fonte canônica representada pelo Markdown exportado equivalente |

Foram calculados SHA-256 de 121 arquivos não audiovisuais. Os 11 vídeos foram controlados por caminho e tamanho porque são brutos, somam mais de 2 GB e não pertencem ao repositório de contexto. O digest do inventário normalizado (`caminho + hash`, ou `caminho + tamanho` para vídeo) é:

`a9ea787c3581b615f278f7e8306b49dc410628d02758da6450b928a9cae4e2c1`

## Regra de cobertura

Uma fonte está coberta quando sua informação muda ou confirma pelo menos uma ideia central, decisão, limite, módulo, critério ou item de histórico. Cobertura não significa copiar o arquivo. Dados pessoais, comerciais, financeiros, documentos de clientes, desenhos técnicos, gravações e rastros internos permanecem fora do Git.

## Famílias e destino semântico

| Grupo | Fontes no Drive | Ideias centrais | Destino principal | Tratamento |
|---|---|---|---|---|
| G-01 Diagnóstico e reuniões | DMO; Sales Call; Kickoff Call; índices e transcrições | IC-01, IC-02, IC-05, IC-08, IC-09, IC-11 | `objetivo.md`, `combinados.md`, `ideias-centrais.*` | Fatos e decisões consolidados; dados comerciais e pessoais omitidos |
| G-02 Escopo e autoria | Escopo base/definitivo; requisitos; revisão; análise crítica; análise do consultor | IC-01 a IC-12 | `ideias-centrais.*`, `limites.md`, `decisoes.json`, `projeto.json` | Precedência e status preservados; metodologia interna não reproduzida |
| G-03 Plano e critérios | Fases; SPECs; tasks; contrato técnico; matriz; histórico pré-Skip | IC-02, IC-03, IC-08, IC-09, IC-10, IC-11 | `produto/modulos*`, `validacao/criterios.json`, `validacao/matriz-legado.json` | Critérios e UUIDs preservados; instruções antigas não reativadas |
| G-04 Setup do assistente | Identidade, soul, user, conectores, agentes e loops | IC-11, IC-12 | `ideias-centrais.*`, contrato modular e estado único | Capacidades registradas; nenhum conector, agente ou loop ativado |
| G-05 Planilhas operacionais | 11 arquivos de lista, peso, reações, kickoff e suprimentos | IC-02, IC-03, IC-04, IC-05, IC-08 | `dicionario.md`, `limites.md`, IC-03/04/05/08 | Esquemas e variações incorporados; clientes, endereços, preços e linhas reais excluídos |
| G-06 Desenhos e PDFs | 22 PDFs de comparativo, contrato/e-mail, modelos, plantas e detalhes | IC-02, IC-03, IC-04 | IC-03/04 e regras de revisão | Existência, família, identidade e revisão incorporadas; binários excluídos |
| G-07 Vídeos de processo | Projetos 1/2; abertura de OC; Etapas 01, 02, 04.1, 04.2 e 05 | IC-02 a IC-09 | `processo-atual.md` e `ideias-centrais.*` | Oito vídeos representados por análises correspondentes |
| G-08 Gravações de reunião | Sales 28/08; Kickoff 18/09; Consultoria 05/10 | IC-01, IC-02, IC-08, IC-11 | atas/transcrições derivadas, escopo e autoria validada | Sales e Kickoff têm transcrição; Consultoria é representada pelos artefatos aprovados de 05/10 |
| G-09 Estado e auditoria | `STATUS.md`, `changelog.md`, checks, revisões, memória e runs | IC-10, IC-11 | `STATUS.md`, `changelog.md`, estado único e decisões | Estado vigente preservado; payloads internos não viram contexto operacional |

## Cobertura dos vídeos

| Vídeo bruto | Representação usada |
|---|---|
| Gravação Sales Call 28/08 | `Sales Call/01-transcricao.md`, ata, decisões e insights |
| Gravação Kickoff 18/09 | `Kickoff Call/01-transcricao.md`, ata, decisões, fluxos e insights; transcrição duplicada na pasta de contexto |
| Gravação Consultoria 05/10 | Escopo definitivo v2, análise do consultor, check de aprovação, SPECs v2 e changelog da mesma data |
| Projetos 1 | `Analise - 1 MAPEAMENTO DOS PROCESSOS - PROJETOS 1.md` |
| Projetos 2 | `Analise - 2 MAPEAMENTO DOS PROCESSOS - PROJETOS 2.md` |
| Abertura de Pedido de Compra | `Analise - 3 MAPEAMENTO DOS PROCESSOS - Abertura_Pedido_Compra.md` |
| Etapa 01 | `Analise - Etapa 01.md` |
| Etapa 02 | `Analise - Etapa 02.md` |
| Etapa 04.1 | `Analise - Etapa04.1AbertuoOC.md` |
| Etapa 04.2 | `Analise - Etapa04.2.md` |
| Etapa 05 | `Analise - Etapa05.md` |

## Variações documentais confirmadas

As planilhas não compartilham um esquema único. A auditoria encontrou, entre outras, estas famílias:

- listas de telhas e painéis com marca, quantidade, descrição, acabamento, largura, espessura e comprimento;
- ordem de produção e conferência de arremates com corte, dobra, carregamento e pesos calculados;
- resumos de peso com seção, comprimento, peso unitário, subtotal, aço e perfil;
- tabela de reações estruturais com revisão, carregamentos, forças e momentos;
- kickoff de obra com campos cadastrais, comerciais, financeiros e administrativos;
- planilha de suprimentos com item, quantidade, unidade, valor unitário e total;
- arquivo de resumo de processo com etapa, atividade, área responsável e nível de detalhe.

Essa diversidade fundamenta IC-03: a solução deve adaptar o mapeamento por família, preservar o original e impedir conversões silenciosas. Não há autorização para um parser universal.

## Lacunas que permanecem visíveis

- A gravação de 05/10 não possui transcrição independente no Drive; sua cobertura deriva dos documentos aprovados na própria data.
- PDFs técnicos predominantemente gráficos não foram convertidos em dados de engenharia. Eles comprovam famílias, identidade e revisão, mas não autorizam extração de cálculo, fabricação ou aprovação técnica.
- Métricas de tempo extraídas dos vídeos descrevem a gravação, não o processo real. Permanecem evidência exploratória, não baseline oficial.
- Integrações com SIGO, SharePoint/OneDrive, WhatsApp, e-mail, CAD/BIM e Skip não foram tecnicamente verificadas por esta auditoria.

## Critério para afirmar completude

O repositório contém o contexto do Drive quando:

1. as 12 ideias centrais cobrem o resultado, a jornada, os objetos, as decisões, as exceções e os limites observados;
2. cada família de fonte aparece na matriz acima e aponta para um destino semântico;
3. módulos e critérios preservam os recortes executáveis já aprovados;
4. lacunas e inferências continuam explícitas;
5. nenhum bruto ou dado real precisa ser publicado para o contexto fazer sentido.

