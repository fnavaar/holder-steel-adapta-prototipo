# Função candidata — consultar obra e documentos

`FUN-OBRA-CONSULTA` continua **proposta**. Este registro permite avançar o co-design, não declara a função aceita nem autoriza implementação.

## Decisão de acesso aprovada (09/10/2026)

Navaar aprovou que o usuário de Planejamento autorizado para uma obra consulte, em **somente leitura**, dados comerciais/financeiros detalhados e documentos/anexos daquela obra. Obras não autorizadas não aparecem nem são acessíveis. A autorização deve ser aplicada na UI e no servidor/API, histórico, downloads e anexos. Outros perfis operacionais não recebem essa ampliação.

**Não inclui:** criar, editar ou excluir dados; aprovar ou alterar contratos, compras, projetos ou lançamentos financeiros; ativar permissões ou usar dados reais. Fonte: `D-PLANEJAMENTO-LEITURA` em `contexto/decisoes.json` e [issue #2](https://github.com/fnavaar/holder-steel-adapta-prototipo/issues/2).

## Continuidade do co-design

O co-design da função pode continuar agora, sem bloqueio global pela revisão de acesso. A obra/documentos do piloto e o vínculo usuários↔obras são insumos a coletar no desenho da jornada e do plano do incremento; enquanto não forem registrados, não se ativa acesso real, mas as partes independentes podem avançar.

A regra separada do modal [issue #1](https://github.com/fnavaar/holder-steel-adapta-prototipo/issues/1) continua válida: somente a pessoa que dará o OK daquela área atualiza a observação da pendência; isso não concede edição geral do card/documentos; preservar autoria e histórico.

## Aceite e execução

`status` permanece `proposta`; `confirmed_by` e `confirmed_at` permanecem nulos até aceite explícito do Champion Felipe Farias. Nenhuma implementação, ativação no Skip ou teste humano é alegado.
