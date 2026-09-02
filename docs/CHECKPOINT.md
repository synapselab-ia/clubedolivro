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
- consolidação: **em andamento — 4/6 artefatos-base concluídos**
- artefatos concluídos:
  - `synthesis/STRUCTURE.md`
  - `synthesis/CHARACTERS.md`
  - `synthesis/THEMES.md`
  - `synthesis/SYMBOLS.md`
- próximo artefato: `synthesis/KEY_PASSAGES.md`

## GLOBAL_RULES

- O repositório é a memória persistente das análises.
- Cada livro possui seu próprio `STATUS.md`.
- A obra é analisada incrementalmente antes da síntese final.
- Evidências e hipóteses devem permanecer distinguíveis.
- PDF/EPUB integral não deve ser publicado enquanto o repositório estiver público.
- Armazenar um PDF/EPUB no GitHub não garante que o conector da IA consiga ler o binário; `BOOK.md` distingue `STORAGE_SOURCE` e `READABLE_SOURCE`.

## LAST_COMPLETED_ACTION

Executada **somente a quarta ação de `CONSOLIDATE`** para *Flores para Algernon*:

- relidos `AGENTS.md`, este checkpoint, `BOOK.md`, `STATUS.md`, `docs/SYNTHESIS_PROTOCOL.md`, `synthesis/STRUCTURE.md`, `synthesis/CHARACTERS.md`, `synthesis/THEMES.md` e `analysis/01.md` a `analysis/10.md`;
- confirmado antes da execução que `synthesis/SYMBOLS.md` não existia;
- criado e verificado `books/flores-para-algernon/synthesis/SYMBOLS.md`;
- `STATUS.md` atualizado marcando **somente `SYMBOLS.md`** como novo artefato concluído;
- nenhum artefato de passagens-chave, interpretações, auditoria ou síntese crítica foi criado.

### Símbolos fortemente sustentados

- **labirinto / caminhos / becos sem saída / choques** — aparato experimental que passa a organizar impasses afetivos, morais e científicos;
- **gaiola / jaula / contenção** — controle experimental, trauma familiar e poder institucional;
- **janela / dentro-fora** — exclusão, proximidade sem acesso e continuidade entre estados de Charlie;
- **flores / túmulo de Algernon** — memória, luto e cuidado depois da utilidade experimental.

### Motivos recorrentes

- antigo Charlie como observador/duplo, sem estatuto de personagem independente;
- espelho/reflexo;
- portas/fechaduras/acesso;
- faca/sangue e ameaça corporal;
- livros/leitura/escrita/Relatórios de Progresso;
- luz/escuridão/visão;
- amuletos/sorte/pensamento mágico;
- sintomas corporais de trauma;
- gravações/filmes/fotografias/documentação;
- comida/recompensa/condicionamento;
- tempo como contagem regressiva.

### Hipóteses simbólicas rebaixadas

- ampulheta/areia — `MEDIUM`;
- sombra no sonho da montanha — `LOW/MEDIUM`;
- “três ratos cegos” — `LOW`;
- medalhão/objetos brilhantes — `LOW/MEDIUM`;
- reflexo de Algernon no toalete — `LOW`.

### Salvaguardas simbólicas

- Algernon não foi reduzido a símbolo: permanece personagem, ser vivo e série empírica; o paralelo com Charlie foi classificado como estrutural `HIGH`;
- Warren e Padaria Donner não foram convertidos em símbolos unívocos;
- os Relatórios de Progresso foram tratados principalmente como dispositivo/motivo formal;
- a relação entre epígrafe de Platão e luz/escuridão continua aberta para auditoria;
- o retorno dos amuletos registra circularidade cognitiva, não reset humano perfeito;
- padrões locais ou ambíguos foram mantidos com confiança reduzida.

### Hipótese simbólica provisória

`INTERPRETATION — HIGH, A AUDITAR`: o sistema imagético mais consistente da obra organiza **controle, acesso e continuidade**. Labirinto, gaiola, janela/porta/espelho, escrita, trauma corporal e flores reapresentam por vias diferentes os conflitos de autonomia, identidade, pertencimento e dignidade.

## NEXT_ACTION

Ler `docs/SYNTHESIS_PROTOCOL.md`, `books/flores-para-algernon/STATUS.md`, `books/flores-para-algernon/synthesis/STRUCTURE.md`, `synthesis/CHARACTERS.md`, `synthesis/THEMES.md`, `synthesis/SYMBOLS.md` e `books/flores-para-algernon/analysis/01.md` a `analysis/10.md`.

Executar **somente a quinta ação de `CONSOLIDATE`**:

- criar `books/flores-para-algernon/synthesis/KEY_PASSAGES.md`;
- selecionar momentos de maior valor analítico distribuídos ao longo da obra;
- registrar para cada momento localização verificável, paráfrase/contexto e função, evitando reprodução extensa do texto;
- assegurar cobertura dos grandes arcos já consolidados: desejo inicial, ascensão, descoberta da humilhação, autonomia, expulsão, Chicago, Algernon, identidade, responsabilidade ética, Warren, descoberta científica, reencontro familiar e regressão/final;
- usar somente leitura interna; não iniciar pesquisa externa;
- ao concluir, atualizar `STATUS.md` e este checkpoint marcando somente `synthesis/KEY_PASSAGES.md` como novo artefato concluído;
- **não criar `INTERPRETATIONS.md` na mesma etapa**;
- **não iniciar `AUDIT`, `SYNTHESIZE`, `PERSONALIZE` ou `FINALIZE`**.

## CONTINUATION_COMMAND

`Continue o projeto synapselab-ia/clubedolivro. Leia AGENTS.md e docs/CHECKPOINT.md, siga os documentos canônicos referenciados e execute a NEXT_ACTION sem refazer etapas concluídas.`