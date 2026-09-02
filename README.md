# Clube do Livro — Leitura Assistida por IA

Repositório canônico para análise incremental de livros, síntese crítica e preparação de material para reuniões de clube do livro.

## Objetivo

Transformar cada obra em um dossiê rastreável, produzido em etapas. A IA não deve gerar uma resenha final a partir de memória vaga ou de um resumo único: primeiro analisa a obra em partes, registra evidências, consolida temas/personagens/estrutura, audita as conclusões e só então produz os materiais finais.

## Como usar

1. Leia `AGENTS.md`.
2. Consulte `docs/CHECKPOINT.md`.
3. Para um novo livro, coloque o arquivo-fonte em `books/_inbox/` **somente se o repositório estiver privado**. Caso contrário, mantenha o PDF/EPUB fora do GitHub e forneça-o diretamente à IA.
4. Em uma nova conversa, peça: `Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md e execute a NEXT_ACTION sem refazer etapas concluídas.`

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
- contexto externo.

Sempre que possível, conclusões interpretativas devem apontar para evidências localizáveis na obra ou nas notas parciais.

## Privacidade e direitos autorais

Não publique arquivos integrais de livros protegidos por direitos autorais em repositório público. Os documentos analíticos deste projeto podem ficar no GitHub; o arquivo-fonte deve permanecer privado quando não houver autorização para distribuição.
