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
- estado: `CONSOLIDATE`
- ingestão: concluída
- mapeamento: concluído
- segmentação: concluída em 10 blocos semânticos
- análise parcial: concluída
- segmentos analisados: **10/10**
- consolidação: **em andamento — 3/6 artefatos-base concluídos**
- artefatos concluídos:
  - `synthesis/STRUCTURE.md`
  - `synthesis/CHARACTERS.md`
  - `synthesis/THEMES.md`
- próximo artefato: `synthesis/SYMBOLS.md`

## GLOBAL_RULES

- O repositório é a memória persistente das análises.
- Cada livro possui seu próprio `STATUS.md`.
- A obra é analisada incrementalmente antes da síntese final.
- Evidências e hipóteses devem permanecer distinguíveis.
- PDF/EPUB integral não deve ser publicado enquanto o repositório estiver público.
- Armazenar um PDF/EPUB no GitHub não garante que o conector da IA consiga ler o binário; `BOOK.md` distingue `STORAGE_SOURCE` e `READABLE_SOURCE`.

## LAST_COMPLETED_ACTION

Executada **somente a terceira ação de `CONSOLIDATE`** para *Flores para Algernon*:

- relidos `AGENTS.md`, este checkpoint, `STATUS.md`, `docs/SYNTHESIS_PROTOCOL.md`, `synthesis/STRUCTURE.md`, `synthesis/CHARACTERS.md` e as análises internas necessárias de `analysis/01.md` a `analysis/10.md`;
- confirmado antes da execução que `synthesis/THEMES.md` não existia;
- criado e verificado `books/flores-para-algernon/synthesis/THEMES.md`;
- `STATUS.md` atualizado marcando **somente `THEMES.md`** como novo artefato concluído;
- nenhum artefato de símbolos, passagens-chave, interpretações, auditoria ou síntese crítica foi criado.

### Temas consolidados

O novo artefato registra definição específica, evidências distribuídas, personagens/eventos associados, evolução, tensões/contradições e confiança para:

1. inteligência e valor humano;
2. dignidade, deficiência e estigma;
3. memória, identidade e continuidade pessoal;
4. pertencimento e solidão;
5. ciência, falibilidade e responsabilidade;
6. autonomia e cuidado;
7. inteligência versus maturidade, afeto e sabedoria;
8. trauma, vergonha e sexualidade;
9. tempo, mortalidade e perda;
10. comunicação, linguagem e acesso à experiência.

Também foi mantido **conhecimento, inocência e limite** como tema transversal `MEDIUM/HIGH`, pendente de auditoria antes de eventual promoção ao núcleo estrutural.

### Salvaguardas temáticas

- inteligência não foi tratada como inútil ou intrinsecamente negativa;
- ciência falível não foi equiparada a anticientificismo;
- dignidade/estigma, pertencimento/solidão e autonomia/cuidado foram diferenciados conceitualmente;
- o cuidado permanece ambivalente entre proteção, paternalismo e tutela;
- compreensão intelectual do trauma não foi confundida com resolução emocional/corporal;
- a regressão final foi tratada como severa, porém não como reset uniforme de toda transformação moral e afetiva;
- motivos imagéticos como labirinto, janela, flores, faca e amuletos foram deixados deliberadamente fora da consolidação temática e aguardam `SYMBOLS.md`;
- a relação com a epígrafe de Platão permanece aberta para auditoria e não foi usada como chave totalizante.

### Hipótese temática provisória

`INTERPRETATION — HIGH, A AUDITAR`: a obra investiga o que permanece humano quando capacidade cognitiva, reconhecimento social e autonomia mudam radicalmente. A inteligência amplia conhecimento e liberdade, mas não substitui afeto, dignidade, responsabilidade ou pertencimento; sua perda não elimina automaticamente todos os vínculos e aprendizados produzidos durante a experiência.

## NEXT_ACTION

Ler `docs/SYNTHESIS_PROTOCOL.md`, `books/flores-para-algernon/STATUS.md`, `books/flores-para-algernon/synthesis/STRUCTURE.md`, `books/flores-para-algernon/synthesis/CHARACTERS.md`, `books/flores-para-algernon/synthesis/THEMES.md` e `books/flores-para-algernon/analysis/01.md` a `analysis/10.md`.

Executar **somente a quarta ação de `CONSOLIDATE`**:

- criar `books/flores-para-algernon/synthesis/SYMBOLS.md`;
- registrar somente padrões com suporte razoável, separando **símbolo fortemente sustentado**, **motivo recorrente** e **hipótese simbólica**;
- priorizar para verificação: Algernon como paralelo que excede função simbólica; labirinto; gaiola/jaula; portas/janelas/estar do lado de fora; espelho/reflexo/duplo; flores; faca/sangue; luz/escuridão; tempo/ampulheta/areia; livros/escrita/relatórios; amuletos/sorte; corpo e sintomas recorrentes; gravações/filmes/fotografias; comida/recompensa;
- não transformar automaticamente personagem, tema ou espaço em símbolo; exigir recorrência e função textual;
- preservar níveis de confiança e rebaixar padrões locais ou especulativos;
- usar somente leitura interna; não iniciar pesquisa externa;
- ao concluir, atualizar `STATUS.md` e este checkpoint marcando somente `synthesis/SYMBOLS.md` como novo artefato concluído;
- **não criar `KEY_PASSAGES.md` ou `INTERPRETATIONS.md` na mesma etapa**;
- **não iniciar `AUDIT`, `SYNTHESIZE`, `PERSONALIZE` ou `FINALIZE`**.

## CONTINUATION_COMMAND

`Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md, siga os documentos canônicos referenciados e execute a NEXT_ACTION sem refazer etapas concluídas.`
