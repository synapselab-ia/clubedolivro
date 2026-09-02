# METHODOLOGY — Pipeline Canônica

## Finalidade

Esta metodologia define como transformar uma obra completa em um conjunto de notas persistentes, auditáveis e reutilizáveis, culminando em materiais finais para discussão em clube do livro.

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

Objetivo: transformar a análise crítica em uma opinião alinhada às reações reais do usuário.

Quando possível, coletar reações do usuário sobre:
- ritmo;
- personagens;
- estilo;
- final;
- temas;
- partes favoritas/menos favoritas;
- nota aproximada.

Não inventar preferências pessoais do usuário.

Saída: base para `final/MY_OPINION.md`.

### 8. FINALIZE

Objetivo: gerar materiais de uso prático.

Seguir `docs/FINAL_OUTPUT_PROTOCOL.md`.

Saídas padrão:
- `final/REVIEW.md`;
- `final/MY_OPINION.md`;
- `final/BOOK_CLUB_BRIEF.md`;
- `final/DISCUSSION_QUESTIONS.md`;
- opcionalmente `final/DEEP_DIVE.md`.

### 9. COMPLETE

Um livro só pode ser marcado `COMPLETE` quando:

- todas as partes previstas estiverem analisadas;
- a consolidação existir;
- a auditoria estiver concluída;
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
- o que vem de fontes externas.

### Análise adversarial

A síntese final deve sobreviver a tentativas explícitas de refutação.
