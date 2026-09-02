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
- segmentos analisados: 1/10

## GLOBAL_RULES

- O repositório é a memória persistente das análises.
- Cada livro possui seu próprio `STATUS.md`.
- A obra é analisada incrementalmente antes da síntese final.
- Evidências e hipóteses devem permanecer distinguíveis.
- PDF/EPUB integral não deve ser publicado enquanto o repositório estiver público.
- Armazenar um PDF/EPUB no GitHub não garante que o conector da IA consiga ler o binário; `BOOK.md` distingue `STORAGE_SOURCE` e `READABLE_SOURCE`.

## LAST_COMPLETED_ACTION

Executado **Segmento 01** de *Flores para Algernon* conforme `docs/ANALYSIS_PROTOCOL.md`:

- escopo: pp. 7–24 do PDF;
- período narrativo: 3 a 29 de março;
- artefato criado: `books/flores-para-algernon/analysis/01.md`;
- análise preserva fatos, personagens, arcos, temas, motivos, passagens-chave, níveis de confiança e questões abertas;
- `books/flores-para-algernon/STATUS.md` sincronizado;
- nenhum conteúdo do Segmento 02 foi analisado nesta etapa.

Eixos iniciais rastreados: inteligência como promessa de pertencimento, escrita como medidor do experimento, ironia dramática nas relações da padaria, paralelismo Charlie–Algernon, recuperação de memória, assimetria de poder científico e primeiros sinais de autonomia cognitiva.

## NEXT_ACTION

Ler `books/flores-para-algernon/BOOK.md`, `books/flores-para-algernon/STATUS.md`, `books/flores-para-algernon/analysis/01.md` e `docs/ANALYSIS_PROTOCOL.md`.

Executar **somente o Segmento 02** de *Flores para Algernon*:

- escopo: pp. 25–39 do PDF;
- início: entrada de 30 de março no `Relatório de Progresso 8`;
- fim: conclusão do novo teste de Rorschach em 18 de abril;
- criar `books/flores-para-algernon/analysis/02.md` conforme `templates/book/analysis/PART_TEMPLATE.md`;
- usar a obra real como fonte e `analysis/01.md` como memória de continuidade, registrando página + Relatório/data quando possível;
- ao concluir, atualizar `STATUS.md` e este checkpoint para 2/10 segmentos analisados, sem iniciar o Segmento 03 na mesma etapa.

## CONTINUATION_COMMAND

`Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md, siga os documentos canônicos referenciados e execute a NEXT_ACTION sem refazer etapas concluídas.`
