# CHECKPOINT — Clube do Livro

Este arquivo registra o estado global canônico do projeto.

## PROJECT_STATE

`READY_FOR_FIRST_BOOK`

## ACTIVE_BOOK

`NONE`

## COMPLETED_SETUP

- [x] Repositório inicializado.
- [x] `README.md` criado.
- [x] `AGENTS.md` criado.
- [x] Estrutura documental canônica definida.
- [x] Pipeline de análise definida.
- [x] Template de livro definido.
- [x] Área de entrada de novas obras definida.

## BOOKS

Nenhum livro inicializado ainda.

## GLOBAL_RULES

- O repositório é a memória persistente das análises.
- Cada livro possui seu próprio `STATUS.md`.
- A obra é analisada incrementalmente antes da síntese final.
- Evidências e hipóteses devem permanecer distinguíveis.
- PDF/EPUB integral não deve ser publicado enquanto o repositório estiver público.

## NEXT_ACTION

Aguardar o usuário fornecer o primeiro livro.

Quando isso acontecer:

1. confirmar que a fonte pode ser lida pela IA;
2. identificar título/autor/edição;
3. criar `books/<slug>/` a partir de `templates/book/`;
4. preencher `BOOK.md` e `STATUS.md`;
5. mapear a estrutura real da obra;
6. definir a segmentação semântica;
7. atualizar este checkpoint com `ACTIVE_BOOK` e a próxima ação concreta.

## CONTINUATION_COMMAND

`Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md, siga os documentos canônicos referenciados e execute a NEXT_ACTION sem refazer etapas concluídas.`
