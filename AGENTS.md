# AGENTS.md — Contrato Operacional

Este arquivo é a porta de entrada obrigatória para qualquer IA trabalhando neste repositório.

## 1. Bootstrap obrigatório

Antes de executar qualquer trabalho:

1. Leia este `AGENTS.md` integralmente.
2. Leia `docs/CHECKPOINT.md`.
3. Se houver `ACTIVE_BOOK`, leia `books/<ACTIVE_BOOK>/STATUS.md` e `books/<ACTIVE_BOOK>/BOOK.md`.
4. Leia apenas os protocolos canônicos necessários à `NEXT_ACTION`.
5. Verifique o estado real dos arquivos do repositório antes de assumir que uma etapa está concluída.
6. Execute a `NEXT_ACTION` sem refazer trabalho marcado como concluído, salvo se houver evidência de inconsistência.

## 2. Ordem de autoridade

Em caso de conflito, prevalece esta ordem:

1. pedido explícito atual do usuário;
2. `AGENTS.md`;
3. `docs/CHECKPOINT.md`;
4. `books/<slug>/STATUS.md`;
5. protocolos em `docs/`;
6. templates;
7. notas históricas.

Nunca trate uma mensagem antiga de chat como mais autoritativa que o estado canônico do repositório.

## 3. Objetivo do sistema

Produzir análises literárias bem fundamentadas a partir da obra real, em etapas pequenas e persistentes, permitindo retomada segura entre conversas e redução de alucinações.

A pipeline padrão é:

`INGEST -> MAP -> SEGMENT -> PART_ANALYSIS -> CONSOLIDATE -> AUDIT -> SYNTHESIZE -> PERSONALIZE -> FINALIZE -> COMPLETE`

## 4. Regras de execução

- Não invente conteúdo da obra.
- Não preencha lacunas com memória geral sobre o livro quando a fonte estiver disponível.
- Não confunda fato textual, interpretação, hipótese e contexto externo.
- Não produza a resenha final antes de concluir análise parcial, consolidação e auditoria, salvo ordem explícita do usuário.
- Não altere análises concluídas apenas para uniformizar estilo; preserve rastreabilidade.
- Não avance duas etapas grandes de uma vez se isso impedir registrar checkpoint intermediário confiável.
- Ao terminar uma etapa, atualize o `STATUS.md` do livro e `docs/CHECKPOINT.md` quando houver mudança global relevante.
- Toda `NEXT_ACTION` deve ser concreta, executável e pequena o suficiente para uma próxima conversa assumir sem ambiguidade.
- Toda **nota numérica final** deve seguir `docs/RATING_PROTOCOL.md`; não escolher a nota apenas por impressão global nem inflá-la porque os melhores momentos da obra são muito fortes.
- Notas `9,0+` exigem justificativa excepcional explícita conforme a rubrica; `10,0` deve ser tratado como nota de referência, não como sinônimo de “gostei muito”.

## 5. Política de evidências

Toda afirmação relevante deve ser classificada implicitamente ou explicitamente como uma destas categorias:

- `TEXTUAL_FACT`: acontecimento, descrição ou informação verificável na obra;
- `INTERPRETATION`: leitura sustentada por evidências;
- `HYPOTHESIS`: leitura possível ainda insuficientemente sustentada;
- `EXTERNAL_CONTEXT`: informação proveniente de crítica, história, entrevistas ou outras fontes externas.

Ao registrar evidências, prefira referências localizáveis: parte, capítulo, seção e página quando a paginação for estável.

## 6. Controle de citações

O sistema existe para análise e comentário, não para reproduzir livros. Evite transcrever passagens longas. Registre preferencialmente:

- referência de localização;
- paráfrase fiel;
- função da passagem na análise;
- citação curta apenas quando a formulação exata for importante.

## 7. Divisão da obra

O alvo padrão é aproximadamente 10 partes, mas não corte mecanicamente a cada 10%.

A segmentação deve respeitar, quando possível:

- capítulos;
- partes internas da edição;
- mudanças de narrador;
- arcos narrativos;
- unidades argumentativas;
- cenas ou transições relevantes.

O número final pode variar se isso preservar melhor a estrutura da obra.

## 8. Memória persistente

Os arquivos do repositório são a memória operacional. Não dependa de lembranças do chat para fatos essenciais.

As análises parciais devem ser escritas para que uma IA futura consiga reconstruir a obra sem reler todas as páginas já processadas, mas sem eliminar referências suficientes para auditoria.

## 9. Novo livro

Quando `ACTIVE_BOOK: NONE` e houver uma nova fonte indicada pelo usuário:

1. identifique título, autor, edição e formato quando possível;
2. crie `books/<slug>/` com base em `templates/book/`;
3. preencha `BOOK.md`;
4. defina o estado inicial em `STATUS.md`;
5. registre o livro em `docs/CHECKPOINT.md` como `ACTIVE_BOOK`;
6. execute o protocolo de ingestão/mapeamento antes de iniciar análise narrativa.

## 10. Arquivos PDF/EPUB

Arquivos integrais protegidos por direitos autorais não devem ser publicados em repositório público.

Além disso, o conector GitHub pode não disponibilizar binários PDF/EPUB como texto diretamente para a IA. Portanto:

- o GitHub é a fonte canônica das notas, status e resultados;
- o arquivo original pode ser arquivado em `books/_inbox/` ou `books/<slug>/source/` se o repositório estiver privado;
- quando necessário para leitura efetiva, o usuário deve fornecer o PDF/EPUB diretamente à conversa/File Library;
- registre em `BOOK.md` como a fonte foi disponibilizada.

## 11. Finalização de uma etapa

Antes de encerrar trabalho:

- confira os arquivos criados/alterados;
- confirme que não há contradição óbvia entre `STATUS.md` e os artefatos existentes;
- atualize `NEXT_ACTION`;
- não marque uma etapa como concluída se o artefato esperado não existir.

## 12. Comando de continuidade recomendado

`Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md, siga os documentos canônicos referenciados e execute a NEXT_ACTION sem refazer etapas concluídas.`