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
- consolidação: **em andamento — 2/6 artefatos-base concluídos**
- artefatos concluídos:
  - `synthesis/STRUCTURE.md`
  - `synthesis/CHARACTERS.md`
- próximo artefato: `synthesis/THEMES.md`

## GLOBAL_RULES

- O repositório é a memória persistente das análises.
- Cada livro possui seu próprio `STATUS.md`.
- A obra é analisada incrementalmente antes da síntese final.
- Evidências e hipóteses devem permanecer distinguíveis.
- PDF/EPUB integral não deve ser publicado enquanto o repositório estiver público.
- Armazenar um PDF/EPUB no GitHub não garante que o conector da IA consiga ler o binário; `BOOK.md` distingue `STORAGE_SOURCE` e `READABLE_SOURCE`.

## LAST_COMPLETED_ACTION

Executada **somente a segunda ação de `CONSOLIDATE`** para *Flores para Algernon*:

- relidos `AGENTS.md`, este checkpoint, `BOOK.md`, `STATUS.md`, `docs/SYNTHESIS_PROTOCOL.md`, `synthesis/STRUCTURE.md` e `analysis/01.md` a `analysis/10.md`;
- confirmado antes da execução que `synthesis/CHARACTERS.md` não existia;
- criado e verificado `books/flores-para-algernon/synthesis/CHARACTERS.md`;
- confirmado que `synthesis/THEMES.md` ainda não existe;
- `STATUS.md` atualizado marcando **somente `CHARACTERS.md`** como novo artefato concluído;
- nenhum artefato de temas, símbolos, passagens-chave, interpretações, auditoria ou síntese crítica foi criado.

### Personagens consolidados

O novo artefato registra posição inicial, motivação aparente, conflitos, decisões, transformação, função temática, relações e ambiguidades para:

- Charlie Gordon;
- Algernon;
- Alice Kinnian;
- professor Nemur;
- dr. Strauss;
- Rose Gordon;
- Matt Gordon;
- Norma Gordon;
- Fay Lillman;
- Joe Carp;
- Frank Reilly;
- Gimpy;
- sr. Donner.

Também foram incluídos, apenas pela função estrutural relevante, Burt Selden, dr. Guarino, sr. Winslow, Fanny Birden, tio Herman, sra. Mooney e Meyer Klaus.

### Salvaguardas de caracterização

- o “antigo Charlie” não foi tratado como personagem independente;
- Warren não foi tratado como personagem;
- motivações inferidas foram marcadas como interpretação;
- Nemur permaneceu simultaneamente cientista de mérito real e figura de objetificação/ambição, sem caricatura de vilão;
- Strauss permaneceu relativamente mais explicativo/prudente, mas sem ser transformado em contraponto moral perfeito;
- Rose foi contextualizada sem converter compreensão em absolvição;
- Matt foi mantido entre proteção pontual e ausência prolongada;
- Norma foi consolidada como arco de ressentimento/estigma infantil para tentativa de reparação adulta;
- Joe/Frank/Gimpy tiveram mudança final preservada sem apagar crueldade, rejeição e ambivalências anteriores;
- Algernon foi tratado como ser vivo, personagem funcional e série empírica, evitando antropomorfização indevida.

### Hipótese provisória de personagens

`INTERPRETATION — HIGH, A AUDITAR`: os personagens organizam diferentes formas de reconhecer, negar, instrumentalizar, cuidar ou temer a humanidade de Charlie. A regressão final é severa, mas as análises sustentam que ela não apaga de maneira perfeitamente uniforme todas as transformações afetivas e morais adquiridas durante o experimento.

## NEXT_ACTION

Ler `docs/SYNTHESIS_PROTOCOL.md`, `books/flores-para-algernon/STATUS.md`, `books/flores-para-algernon/synthesis/STRUCTURE.md`, `books/flores-para-algernon/synthesis/CHARACTERS.md` e `books/flores-para-algernon/analysis/01.md` a `analysis/10.md`.

Executar **somente a terceira ação de `CONSOLIDATE`**:

- criar `books/flores-para-algernon/synthesis/THEMES.md`;
- para cada tema central, registrar definição específica na obra, evidências distribuídas, personagens/eventos associados, evolução, tensões/contradições e grau de confiança;
- priorizar inteligência e valor humano; pertencimento/solidão; dignidade/deficiência/estigma; ciência/falibilidade/responsabilidade; autonomia/cuidado; memória/identidade/continuidade pessoal; inteligência versus maturidade/afeição; trauma/vergonha/sexualidade; tempo/mortalidade; comunicação/linguagem;
- separar rigorosamente tema de símbolo/motivo: labirinto, janela, flores, faca, amuletos etc. devem aguardar `SYMBOLS.md` quando sua função for imagética/recorrente;
- usar somente leitura interna; não iniciar pesquisa externa;
- ao concluir, atualizar `STATUS.md` e este checkpoint marcando somente `synthesis/THEMES.md` como novo artefato concluído;
- **não criar `SYMBOLS.md`, `KEY_PASSAGES.md` ou `INTERPRETATIONS.md` na mesma etapa**;
- **não iniciar `AUDIT`, `SYNTHESIZE`, `PERSONALIZE` ou `FINALIZE`**.

## CONTINUATION_COMMAND

`Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md, siga os documentos canônicos referenciados e execute a NEXT_ACTION sem refazer etapas concluídas.`
