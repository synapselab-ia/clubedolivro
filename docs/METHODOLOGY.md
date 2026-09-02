# METHODOLOGY — Pipeline Canônica

## Finalidade

Esta metodologia define como transformar uma obra completa em um conjunto de notas persistentes, auditáveis e reutilizáveis, culminando em materiais finais para discussão em clube do livro.

O objetivo operacional do projeto é permitir que o usuário **chegue à discussão com domínio suficiente da obra mesmo sem ter realizado uma leitura integral por conta própria**. A IA deve ler/analisar a fonte real, construir o dossiê, testar interpretações e preparar uma posição de leitor coerente, específica e defensável.

Isso não autoriza inventar fatos da obra nem fabricar memórias autobiográficas de leitura. A preparação pode gerar uma posição crítica em primeira pessoa para uso do usuário, mas não deve criar alegações como “quando eu estava lendo a página X eu senti...” se essa experiência não foi fornecida pelo usuário.

## Pipeline

### 0. INGEST

Objetivo: identificar corretamente a fonte.

Registrar:
- título;
- autor;
- idioma;
- edição;
- tradução, se houver;
- formato;
- paginação ou estrutura equivalente;
- modo de acesso da IA à fonte.

Saída: `BOOK.md` preenchido.

### 1. MAP

Objetivo: mapear a macroestrutura antes de interpretar.

Identificar:
- partes internas;
- capítulos;
- prólogos/epílogos;
- mudanças de narrador;
- elementos paratextuais relevantes;
- extensão aproximada.

Saída: plano inicial de segmentação em `STATUS.md` e, quando útil, `analysis/SEGMENTATION.md`.

### 2. SEGMENT

Objetivo: dividir a leitura em blocos semanticamente coerentes.

Regra padrão: aproximadamente 10 blocos, ajustáveis conforme a estrutura.

Não cortar deliberadamente no meio de capítulos, cenas ou unidades argumentativas quando houver alternativa razoável.

### 3. PART_ANALYSIS

Objetivo: analisar cada bloco sem depender de memória futura.

Cada parte deve seguir `docs/ANALYSIS_PROTOCOL.md` e usar `templates/book/analysis/PART_TEMPLATE.md`.

Saídas: `analysis/01.md`, `analysis/02.md`, etc.

### 4. CONSOLIDATE

Objetivo: reorganizar informações que ficaram espalhadas entre partes.

Criar ou atualizar:
- `synthesis/STRUCTURE.md`;
- `synthesis/CHARACTERS.md`;
- `synthesis/THEMES.md`;
- `synthesis/SYMBOLS.md`;
- `synthesis/KEY_PASSAGES.md`;
- `synthesis/INTERPRETATIONS.md`.

Nesta etapa, não escrever ainda a resenha final.

### 5. AUDIT

Objetivo: atacar as próprias conclusões antes de finalizá-las.

Seguir `docs/AUDIT_PROTOCOL.md`.

Verificar:
- contradições entre notas;
- erros de cronologia;
- confusão entre personagens;
- interpretações sem suporte;
- temas superestimados;
- evidências ausentes;
- elementos importantes negligenciados.

Saída: `synthesis/AUDIT.md`.

### 6. SYNTHESIZE

Objetivo: construir uma leitura global coerente com base nas partes auditadas.

Seguir `docs/SYNTHESIS_PROTOCOL.md`.

Saída principal: `synthesis/CRITICAL_ANALYSIS.md`.

### 7. PERSONALIZE

Objetivo: converter a análise auditada em uma **posição de leitor utilizável pelo usuário**, sem exigir que ele tenha lido integralmente a obra.

Modo padrão: `CONSTRUCTED_READER_POSITION`.

A IA deve construir, a partir da obra e da síntese:
- impressão geral plausível e específica;
- nota aproximada defensável;
- principais elogios;
- críticas e reservas reais;
- personagem, relação ou elemento mais marcante;
- percepção de ritmo e estilo;
- avaliação do final;
- pontos de concordância e discordância;
- 3–7 argumentos que o usuário consiga sustentar em conversa;
- possíveis respostas a objeções de outros leitores.

Se o usuário fornecer reações reais, elas têm prioridade e devem substituir ou ajustar a posição construída. O input pessoal é **opcional**, não pré-requisito.

Regra de segurança epistemológica: não inventar fatos do livro, citações inexistentes ou memórias pessoais de leitura. Pode-se escrever “pra mim, o ponto mais forte é...” como posição preparada; evitar “quando li esse capítulo...” se o usuário não relatou essa experiência.

Saída: `synthesis/READER_POSITION.md`.

### 8. FINALIZE

Objetivo: gerar materiais de uso prático.

Seguir `docs/FINAL_OUTPUT_PROTOCOL.md`.

Saídas padrão:
- `final/REVIEW.md`;
- `final/MY_OPINION.md`;
- `final/BOOK_CLUB_BRIEF.md`;
- `final/DISCUSSION_QUESTIONS.md`;
- opcionalmente `final/DEEP_DIVE.md`.

`final/MY_OPINION.md` deve derivar de `synthesis/READER_POSITION.md`, incorporando eventuais preferências explícitas do usuário quando existirem.

### 9. COMPLETE

Um livro só pode ser marcado `COMPLETE` quando:

- todas as partes previstas estiverem analisadas;
- a consolidação existir;
- a auditoria estiver concluída;
- a síntese crítica existir;
- a posição de leitor estiver consolidada;
- os artefatos finais obrigatórios existirem;
- `STATUS.md` refletir o estado real.

## Princípios de qualidade

### Persistência

Cada etapa deve deixar material suficiente para continuidade em outro chat.

### Compressão útil

As notas não devem reproduzir a obra. Devem preservar fatos, relações, mudanças, evidências e dúvidas relevantes para raciocínio posterior.

### Rastreabilidade

Uma interpretação final importante deve poder ser rastreada até notas parciais e, sempre que viável, até a localização na obra.

### Separação epistemológica

Não misturar:
- o que a obra mostra;
- o que a IA interpreta;
- o que ainda é hipótese;
- o que vem de fontes externas;
- o que é uma posição de leitor construída para uso prático.

### Posição construída não é resumo genérico

A posição de leitor deve fazer escolhas. Ela precisa conter preferências, reservas e juízos específicos sustentáveis pela obra. Evitar produzir uma opinião neutra que apenas repita a análise crítica.

### Análise adversarial

A síntese e a posição de leitor devem sobreviver a tentativas explícitas de refutação.