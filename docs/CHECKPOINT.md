# CHECKPOINT — Clube do Livro

Este arquivo registra o estado global canônico do projeto.

## PROJECT_STATE

`READY_FOR_FIRST_BOOK`

## REPOSITORY_VISIBILITY

`PUBLIC`

## SOURCE_UPLOAD_STATUS

`DO_NOT_UPLOAD_COPYRIGHTED_PDF_EPUB_WHILE_PUBLIC`

## ACTIVE_BOOK

`NONE`

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

Nenhum livro inicializado ainda.

## GLOBAL_RULES

- O repositório é a memória persistente das análises.
- Cada livro possui seu próprio `STATUS.md`.
- A obra é analisada incrementalmente antes da síntese final.
- Evidências e hipóteses devem permanecer distinguíveis.
- PDF/EPUB integral não deve ser publicado enquanto o repositório estiver público.
- Armazenar um PDF/EPUB no GitHub não garante que o conector da IA consiga ler o binário; `BOOK.md` deve distinguir `STORAGE_SOURCE` e `READABLE_SOURCE`.

## NEXT_ACTION

Aguardar o primeiro livro.

Antes de colocar PDF/EPUB integral protegido no GitHub, o usuário deve tornar o repositório privado. Alternativamente, pode fornecer o arquivo diretamente ao ChatGPT/File Library e manter apenas as análises no GitHub.

Quando a fonte estiver disponível em formato efetivamente legível pela IA:

1. identificar título/autor/edição;
2. criar `books/<slug>/` a partir de `templates/book/`;
3. preencher `BOOK.md` e `STATUS.md`;
4. mapear a estrutura real da obra;
5. definir a segmentação semântica;
6. atualizar este checkpoint com `ACTIVE_BOOK` e a próxima ação concreta.

## CONTINUATION_COMMAND

`Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md, siga os documentos canônicos referenciados e execute a NEXT_ACTION sem refazer etapas concluídas.`
