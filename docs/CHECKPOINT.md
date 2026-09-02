# CHECKPOINT — Clube do Livro

Este arquivo registra o estado global canônico do projeto.

## PROJECT_STATE

`BOOK_ACTIVE`

## REPOSITORY_VISIBILITY

`PUBLIC`

## SOURCE_UPLOAD_STATUS

`SOURCE_AVAILABLE_VIA_CHATGPT_FILE_LIBRARY`

O PDF integral não deve ser enviado ao GitHub enquanto o repositório permanecer público.

## ACTIVE_BOOK

`flores-para-algernon`

## COMPLETED_SETUP

- [x] Repositório inicializado.
- [x] `README.md` criado.
- [x] `AGENTS.md` criado.
- [x] Estrutura documental canônica definida.
- [x] Pipeline de análise definida.
- [x] Protocolos de análise, síntese, auditoria, opinião e pesquisa externa definidos.
- [x] Template completo de livro definido.
- [x] Área de entrada de novas obras definida.
- [x] Pasta `source/` prevista no template de cada livro.
- [x] Estrutura verificada no repositório.

## BOOKS

### `flores-para-algernon`

- título: *Flores para Algernon*
- autor: Daniel Keyes
- edição analisada: Aleph, edição eletrônica brasileira de 2018, tradução de Luisa Geisler
- fonte legível: PDF fornecido diretamente ao ChatGPT/File Library
- estado: `PART_ANALYSIS`
- ingestão: concluída
- mapeamento: concluído
- segmentação: concluída em 10 blocos semânticos
- segmentos analisados: 0/10

## GLOBAL_RULES

- O repositório é a memória persistente das análises.
- Cada livro possui seu próprio `STATUS.md`.
- A obra é analisada incrementalmente antes da síntese final.
- Evidências e hipóteses devem permanecer distinguíveis.
- PDF/EPUB integral não deve ser publicado enquanto o repositório estiver público.
- Armazenar um PDF/EPUB no GitHub não garante que o conector da IA consiga ler o binário; `BOOK.md` distingue `STORAGE_SOURCE` e `READABLE_SOURCE`.

## LAST_COMPLETED_ACTION

O primeiro livro foi inicializado conforme `AGENTS.md`:

1. fonte e edição identificadas;
2. `books/flores-para-algernon/` criado;
3. `BOOK.md` e `STATUS.md` preenchidos;
4. estrutura real da obra mapeada (17 Relatórios de Progresso);
5. narrativa dividida em 10 segmentos semânticos documentados em `analysis/SEGMENTATION.md`;
6. fonte mantida fora do GitHub público e registrada em `source/SOURCE_NOTES.md`.

## NEXT_ACTION

Ler `books/flores-para-algernon/BOOK.md`, `books/flores-para-algernon/STATUS.md` e `docs/ANALYSIS_PROTOCOL.md`.

Executar **somente o Segmento 01** de *Flores para Algernon*:

- escopo: pp. 7–24 do PDF;
- início: `Relatório de Progresso 1`, 3 de março;
- fim: conclusão da entrada de 29 de março no `Relatório de Progresso 8`;
- criar `books/flores-para-algernon/analysis/01.md` conforme `templates/book/analysis/PART_TEMPLATE.md`;
- usar a obra real como fonte, registrando página + Relatório/data quando possível;
- ao concluir, atualizar `STATUS.md` e este checkpoint para 1/10 segmentos analisados, sem iniciar o Segmento 02 na mesma etapa.

## CONTINUATION_COMMAND

`Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md, siga os documentos canônicos referenciados e execute a NEXT_ACTION sem refazer etapas concluídas.`
