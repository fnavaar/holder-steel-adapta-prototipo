# Padrões de experiência

## 6. UI/UX: duas experiências distintas

### Experiência de construir (Maestro/portal)

Uma entrada clara, módulo ativo, resultado desejado, prévia e próximo passo. A conversa pergunta somente o necessário para a função atual. Mostrar progresso por comportamento demonstrado, não por número de arquivos ou prompts. Separar “design aprovado”, “construído”, “verificado” e “aceito”.

### Experiência de usar (sistema Holder no Skip)

**Arquitetura de navegação candidata:** visão geral de obras → obra selecionada → resumo/documentos/pendências/Lista Master; revisões, compras, recebimentos e financeiro conforme módulos realmente construídos. Função futura não aparece como botão que simula funcionamento; ocultar ou rotular claramente como planejada.

**Padrões propostos:**
- Obra/escopo/revisão sempre visíveis no contexto da tela.
- Ação principal clara por tela; tarefas relacionadas agrupadas.
- Campos em linguagem da Holder, exemplos e ajuda contextual; obrigatório versus não informado explícitos.
- Planejamento pode consultar, somente para leitura, detalhes comerciais/financeiros e documentos/anexos apenas quando o usuário estiver autorizado para aquela obra; outras obras e perfis operacionais não recebem esses dados. Aplicar o mesmo controle na UI, autorização server-side/API, histórico, downloads e anexos; mutações e decisões financeiras permanecem negadas.
- Listas com busca/filtros úteis, preservando contexto ao abrir e voltar.
- Formulários com salvamento confirmado, validação próxima do campo e aviso de edição concorrente.
- Estados de carregamento, vazio, erro, sem permissão, dado incompleto e sucesso distinguíveis.
- Confirmação especial para ação destrutiva/reversão; nova tentativa não duplica registro.
- Acessibilidade verificável: teclado, foco, labels, erros anunciáveis, contraste e zoom; responsividade conforme dispositivos realmente usados, sem impor mobile a toda tela por suposição.
- Densidade adaptada ao trabalho: escritório pode precisar de tabelas; campo, conferência simples. Validar com usuários e exemplos.
- Informação de fonte, atualização e cobertura junto aos números; sem falso “tempo real”.

**Prova de UX:** cenário com usuário/objetivo, tarefa que consegue concluir, pontos de dúvida/erro e caminho de retorno. Medir tempo ativo, conclusão, esclarecimentos e retrabalho no piloto. Design “mais bonito” não é critério suficiente. Preferências de cores/componentes são candidatas até validar identidade visual; não inventar design system oficial da Holder.



As diretrizes de UX são propostas para confirmar no contrato de função; não introduzem critérios legados retroativos. Testar teclado/foco/labels, mensagens de erro e responsividade nos dispositivos da jornada real. Não declarar conformidade formal sem teste.
