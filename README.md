# Clube do Livro — Leitura Assistida por IA

Repositório canônico para análise incremental de livros, síntese crítica e preparação de material para reuniões de clube do livro.

## Objetivo

Transformar cada obra em um dossiê rastreável, produzido em etapas, para que o usuário consiga **discutir a obra com domínio e segurança mesmo sem ter realizado uma leitura integral por conta própria**.

A IA não deve gerar uma resenha final a partir de memória vaga ou de um resumo único: primeiro analisa a obra real em partes, registra evidências, consolida temas/personagens/estrutura, audita as conclusões, constrói uma posição de leitor defensável e só então produz os materiais finais.

A posição preparada pode ser usada em primeira pessoa e conter nota, elogios, críticas e interpretações. O projeto não deve, porém, inventar fatos da obra ou memórias autobiográficas de leitura como “quando eu li esse capítulo...”.

## Como usar

1. Leia `AGENTS.md`.
2. Consulte `docs/CHECKPOINT.md`.
3. Para um novo livro, coloque o arquivo-fonte em `books/_inbox/` **somente se o repositório estiver privado**. Caso contrário, mantenha o PDF/EPUB fora do GitHub e forneça-o diretamente à IA.
4. Em uma nova conversa, peça: `Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md e execute a NEXT_ACTION sem refazer etapas concluídas.`

## Fluxo prático

A pipeline canônica é:

`INGEST -> MAP -> SEGMENT -> PART_ANALYSIS -> CONSOLIDATE -> AUDIT -> SYNTHESIZE -> PERSONALIZE -> FINALIZE -> COMPLETE`

Na etapa `PERSONALIZE`, o modo padrão é `CONSTRUCTED_READER_POSITION`: a IA transforma a análise auditada em uma posição crítica utilizável pelo usuário. Reações pessoais do usuário podem calibrar essa posição, mas não são obrigatórias.

## Estrutura

- `AGENTS.md` — contrato operacional para qualquer IA que trabalhe no repositório.
- `docs/` — metodologia e protocolos canônicos.
- `templates/book/` — modelo de estrutura para cada livro.
- `books/_inbox/` — área de entrada de novas obras.
- `books/<slug>/` — dossiê persistente de cada livro analisado.

## Princípio central

Toda conclusão relevante deve ser distinguida entre:

- fato textual;
- interpretação;
- hipótese;
- contexto externo;
- posição de leitor construída para uso prático.

Sempre que possível, conclusões interpretativas devem apontar para evidências localizáveis na obra ou nas notas parciais.

## Privacidade e direitos autorais

Não publique arquivos integrais de livros protegidos por direitos autorais em repositório público. Os documentos analíticos deste projeto podem ficar no GitHub; o arquivo-fonte deve permanecer privado quando não houver autorização para distribuição.