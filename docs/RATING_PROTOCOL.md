# RATING_PROTOCOL — Rubrica Crítica de Nota

## Objetivo

Padronizar a atribuição de notas no Clube do Livro e evitar inflação de avaliação.

A nota não deve ser escolhida por impressão global e depois justificada retroativamente. Ela deve resultar de uma **avaliação crítica explícita por dimensões**, realizada depois da auditoria e da síntese da obra.

Modo padrão:

`STRICT_RUBRIC`

Escala final:

`0,0–10,0`, em incrementos de **0,5 ponto**.

Notas **9,0 ou superiores são deliberadamente raras**. Nota 10 não significa apenas “gostei muito”: significa uma obra de referência, excepcional mesmo sob análise adversarial.

---

## 1. Princípio de severidade

Não começar em 10 e descontar defeitos.

Cada dimensão deve ser avaliada independentemente a partir das evidências consolidadas. Méritos extraordinários em uma área não apagam automaticamente falhas relevantes em outra.

A pergunta não é “o livro é bom?”. A pergunta é:

> **quão bem a obra executa aquilo que se propõe, e quão importantes são suas limitações quando examinadas com rigor?**

Preferir uma nota conservadora quando houver dúvida real entre dois níveis.

---

## 2. Dimensões e pesos

A rubrica-base é:

| Dimensão | Peso | O que avaliar |
|---|---:|---|
| Execução formal e estilo | 20% | linguagem, voz, técnica, forma, coerência entre forma e conteúdo |
| Profundidade temática e intelectual | 20% | complexidade, ambiguidade, desenvolvimento dos temas, resistência a leituras simplistas |
| Personagens e relações | 15% | construção, evolução, densidade psicológica, relações e agência |
| Estrutura e ritmo | 15% | organização, progressão, repetição, equilíbrio, transições e controle do ritmo |
| Originalidade e identidade artística | 10% | singularidade da proposta e da execução, sem exigir novidade absoluta de premissa |
| Impacto emocional/estético | 10% | força, memorabilidade e eficácia dos efeitos pretendidos |
| Consistência e fechamento | 10% | sustentação do conjunto, payoff, final e ausência de contradições relevantes |

Total: **100%**.

### Adaptação por gênero

Os pesos são padrão, não uma camisa de força. Em ensaio, poesia, teatro, não ficção ou formas experimentais, uma dimensão pode ser reinterpretada ou redistribuída.

Qualquer redistribuição deve:

- manter 100%;
- ser registrada antes do cálculo final;
- não ser feita para favorecer artificialmente a obra.

---

## 3. Escala interna de cada dimensão

Usar notas de 0 a 10, preferencialmente em incrementos de 0,5.

### 10 — excepcional / referência

Execução extraordinária, de nível referencial, sem fragilidade material relevante naquela dimensão.

### 9 — extraordinário

Muito acima do padrão, com falhas pequenas ou localizadas que não comprometem substancialmente a dimensão.

### 8 — muito bom

Méritos fortes e consistentes, mas com limitações perceptíveis e relevantes.

### 7 — bom

Funciona bem no conjunto, porém possui problemas claros de execução, profundidade ou consistência.

### 6 — razoável / acima do mediano

Tem qualidades reais, mas é irregular e possui limitações importantes.

### 5 — mediano

Equilíbrio aproximado entre acertos e problemas; competente sem se destacar de modo consistente.

### 4 — fraco

Problemas relevantes superam os méritos.

### 3 ou menos — muito fraco

Falhas fundamentais de execução, coerência ou eficácia predominam.

---

## 4. Cálculo

1. atribuir nota a cada dimensão;
2. multiplicar pelo peso;
3. somar os resultados para obter a `RAW_SCORE`;
4. aplicar as regras de teto e severidade;
5. converter para a nota final em incrementos de 0,5.

### Arredondamento

- arredondar para o múltiplo de 0,5 mais próximo;
- em empate exato entre dois múltiplos, arredondar **para baixo**;
- a rubrica pode impor teto inferior ao arredondamento matemático.

Exemplo:

`RAW_SCORE: 8,70` → `FINAL_SCORE: 8,5`.

---

## 5. Regras de teto

O cálculo matemático não basta. Aplicar também estas travas qualitativas.

### Para receber 10,0

A obra deve:

- alcançar nível excepcional/referencial no conjunto;
- não possuir limitação material recorrente identificada pela auditoria;
- não depender de compensação do tipo “é brilhante apesar de uma parte claramente fraca”;
- sustentar defesa explícita de por que merece a nota máxima.

**10,0 deve ser extremamente raro.**

### Para receber 9,5

Exige obra extraordinária, próxima de referência, com apenas fragilidades pequenas e localizadas.

### Para receber 9,0

Exige obra extraordinária no conjunto. Se houver **falha recorrente, seção claramente inferior, problema estrutural importante ou limitação relevante em mais de uma dimensão**, o teto padrão passa a ser **8,5**, salvo defesa excepcional registrada.

### Para receber 8,5

Obra excelente, com grandes méritos e identidade forte, mas com limitações claras o suficiente para impedir classificação como extraordinária.

### Para receber 8,0

Obra muito boa e recomendável, com qualidades fortes, porém problemas relevantes e perceptíveis.

---

## 6. Antiinflacionamento

Antes de fechar qualquer nota ≥ 8,5, responder explicitamente:

1. **Qual é a melhor razão para dar 0,5 ponto a menos?**
2. **Qual dimensão é a mais fraca?**
3. **Os defeitos são realmente pequenos ou estamos perdoando porque os melhores momentos são muito bons?**
4. **Se esta obra receber 9,0, o que ficará reservado para uma obra claramente superior?**

Se essas perguntas revelarem uma limitação material não refletida na nota, recalibrar para baixo.

---

## 7. Nota crítica versus gosto pessoal

Separar:

- `CRITICAL_SCORE` — resultado da rubrica;
- `PERSONAL_ENJOYMENT` — gosto/reação do usuário, quando existir.

Por padrão, a nota publicada nos materiais finais é o **`CRITICAL_SCORE`**, calibrado pelas preferências do usuário apenas quando ele explicitamente quiser uma nota de gosto pessoal.

Uma pessoa pode gostar 10/10 de uma obra e ainda reconhecer uma avaliação crítica 8,0/10, ou o inverso.

No modo `CONSTRUCTED_READER_POSITION`, não inventar uma segunda nota emocional sem necessidade.

---

## 8. Registro obrigatório

Ao concluir `PERSONALIZE`, `synthesis/READER_POSITION.md` deve registrar:

- `RATING_MODE: STRICT_RUBRIC`;
- notas das dimensões;
- `RAW_SCORE`;
- eventual teto aplicado;
- `FINAL_SCORE`;
- 2–5 linhas explicando por que a obra não recebeu 0,5 ponto a mais.

Os seguintes arquivos devem usar a mesma nota final:

- `synthesis/READER_POSITION.md`;
- `final/REVIEW.md`;
- `final/MY_OPINION.md`;
- `final/BOOK_CLUB_BRIEF.md`;
- `STATUS.md`;
- `docs/CHECKPOINT.md`, quando registrar a obra concluída.

---

## 9. Auditoria final da nota

Antes de `COMPLETE`, confirmar:

- [ ] a nota deriva da rubrica, não de impressão vaga;
- [ ] os pesos somam 100%;
- [ ] limitações da auditoria aparecem nas dimensões correspondentes;
- [ ] regras de teto foram consideradas;
- [ ] qualquer nota ≥ 9,0 possui defesa excepcional explícita;
- [ ] a nota é idêntica em todos os artefatos canônicos;
- [ ] não há inflação causada apenas por impacto emocional ou popularidade da obra.

## Veredito

Uma nota alta deve significar alguma coisa.

**8,0 é muito bom. 8,5 é excelente. 9,0 é extraordinário. 9,5 é raríssimo. 10,0 é referência excepcional.**