---
name: construir-por-modulos
description: "Esta skill candidata deve ser usada na Holder Steel quando o usuário pedir criar uma função, melhorar uma tela, desenhar uma jornada ou continuar o módulo no piloto autorizado. Não instalada globalmente."
version: 0.1.0-candidate
---
# Construção assistida por módulos
Ler AGENTS.md da raiz e execucao/estado.json. Usar somente repo/projeto autorizados. Orientar por intenção: entender projeto, desenhar função, desenhar jornada/UI, construir incremento, verificar, corrigir gap, retomar. Esses são territórios de ação, não tools ou slash commands existentes.

Co-desenhar contrato por produto/funcoes/TEMPLATE.md, perguntar insumos ao Champion juntos, recomendar jornada e interface com padrões de produto/ui-ux/padroes.md. Ler contexto e critérios somente pertinentes, mantendo visão funcional do arco. Não carregar 156 arquivos nem usar conhecimento geral para preencher dado operacional desconhecido.

Classificar pedido: dentro do módulo → iterar no recorte autorizado; dado/regra faltante → pergunta ao Champion e partes independentes seguras; fora do ciclo → backlog/consultor. Não converter idéia em implementação automaticamente.

Inspecionar código/preview/versão antes de criar entidade. Preservar modelo Work/migrations e segurança existentes; uma fatia completa, um escritor ativo. Edição externa no Skip exige reconciliação antes de escrever.

Construir somente após autorização concreta, registrar testes reais e estado. Falta de ferramenta não vale teste/RED. Consultor valida comparação antes da devolutiva; Champion testa. Não aprovar gate em nome humano. Corrigir no mesmo módulo; função aceita não fecha fase.

Retomar mesma função e etapa a partir do estado; nunca iniciar task legada por automatismo. Se protocolo modular não foi selecionado no runtime, declarar ausência da ativação, não simular plugin ativo.
