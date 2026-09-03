# PERSONAL_OPINION_PROTOCOL — Construção da Posição de Leitor

## Objetivo

Transformar a análise auditada da obra em uma **posição de leitor específica, plausível e defensável para uso do usuário**, sem exigir que ele tenha realizado a leitura integral por conta própria.

O modo padrão é:

`CONSTRUCTED_READER_POSITION`

O usuário pode fornecer reações pessoais, mas isso é opcional. Quando existirem, elas prevalecem sobre preferências geradas pela IA.

Toda nota numérica deve seguir `docs/RATING_PROTOCOL.md` no modo padrão `STRICT_RUBRIC`.

## Princípio central

A IA deve construir uma posição que uma pessoa bem informada consiga sustentar em conversa porque conhece:

- fatos importantes do enredo;
- arcos dos personagens;
- escolhas formais;
- temas centrais;
- ambiguidades;
- pontos fortes e limitações reais da obra.

A posição não deve ser um resumo neutro. Precisa fazer escolhas avaliativas.

A nota não deve ser escolhida intuitivamente para depois receber uma justificativa. Primeiro avaliar méritos e limitações por dimensão; depois calcular e auditar a nota.

## Inputs obrigatórios

- `synthesis/AUDIT.md`;
- `synthesis/CRITICAL_ANALYSIS.md`;
- `docs/RATING_PROTOCOL.md`;
- quando necessário, `STRUCTURE.md`, `CHARACTERS.md`, `THEMES.md`, `KEY_PASSAGES.md` e análises parciais.

## Inputs opcionais do usuário

Se disponíveis, usar para calibrar:

- gêneros e estilos de que costuma gostar;
- reações reais a trechos que tenha lido;
- personagem que chamou atenção;
- tolerância a ritmo lento/rápido;
- preferência por finais trágicos, abertos etc.;
- nota que queira atribuir.

A ausência desses inputs **não bloqueia `PERSONALIZE`**.

Se o usuário fornecer uma nota de gosto pessoal, manter explícita a diferença entre `CRITICAL_SCORE` e `PERSONAL_ENJOYMENT` quando elas não coincidirem.

## Procedimento

1. extrair da síntese 3–5 méritos fortes da obra;
2. identificar 1–3 limitações ou reservas defensáveis;
3. pontuar as dimensões definidas em `docs/RATING_PROTOCOL.md`;
4. calcular o `RAW_SCORE` ponderado;
5. aplicar regras de teto, severidade e anti-inflacionamento;
6. definir o `FINAL_SCORE` em incrementos de 0,5;
7. responder explicitamente por que a obra não merece 0,5 ponto a mais, especialmente se `FINAL_SCORE >= 8,5`;
8. escolher uma avaliação geral coerente com a nota calculada;
9. selecionar personagem, relação ou elemento mais marcante;
10. avaliar ritmo e estilo de forma específica;
11. formular posição sobre o final;
12. escolher ao menos uma interpretação com a qual a posição construída concorda fortemente;
13. escolher ao menos uma nuance, crítica ou discordância para evitar opinião artificialmente perfeita;
14. preparar argumentos curtos que possam ser usados em conversa;
15. registrar contra-argumentos plausíveis e respostas defensáveis;
16. salvar em `synthesis/READER_POSITION.md`.

## Estrutura mínima de `READER_POSITION.md`

- `MODE`: `CONSTRUCTED_READER_POSITION` ou `USER_CALIBRATED_READER_POSITION`;
- `RATING_MODE: STRICT_RUBRIC`;
- avaliação geral;
- notas por dimensão e pesos;
- `RAW_SCORE`;
- teto qualitativo, quando aplicável;
- `FINAL_SCORE`;
- justificativa de por que não recebeu 0,5 ponto a mais;
- o que mais funciona;
- o que menos funciona / reservas;
- personagem/relação/elemento mais marcante;
- ritmo;
- estilo;
- final;
- posição sobre temas/conflitos centrais;
- argumentos de conversa;
- discordâncias plausíveis;
- perguntas que o usuário pode devolver ao grupo;
- afirmações a evitar por serem factualmente frágeis ou excessivas.

## Regra de voz

A posição pode ser redigida em primeira pessoa para ser naturalmente reutilizável, por exemplo:

- “Pra mim, o que mais funciona no livro é...”;
- “Eu acho que a relação com Algernon é mais importante do que o romance com Alice porque...”;
- “Minha principal reserva é...”;

Isso é uma **posição crítica preparada**, não uma alegação de memória autobiográfica.

## Regra de severidade

A interpretação verbal da nota deve seguir a escala canônica:

- `8,0` — muito bom;
- `8,5` — excelente;
- `9,0` — extraordinário;
- `9,5` — raríssimo / próximo de referência;
- `10,0` — referência excepcional.

Não usar 9 ou 10 como sinônimos genéricos de “gostei bastante”. Uma falha recorrente, uma seção claramente mais fraca ou problemas relevantes em múltiplas dimensões devem reduzir materialmente a nota.

## Proibições

Não:

- inventar fatos da obra;
- criar citações inexistentes;
- afirmar que o usuário leu uma passagem específica;
- inventar experiências sensoriais ou cronológicas de leitura, como “quando cheguei nesse capítulo fiquei...”;
- transformar hipótese rejeitada pela auditoria em opinião factual;
- produzir uma posição tão genérica que pudesse servir para qualquer livro;
- escolher a nota antes de aplicar a rubrica;
- elevar a nota apenas por popularidade, reputação ou impacto emocional isolado.

## Critério de conclusão

`PERSONALIZE` está concluído quando existe um `synthesis/READER_POSITION.md` coerente com a auditoria, com rubrica de nota registrada e suficientemente específico para alimentar `final/MY_OPINION.md` e `final/BOOK_CLUB_BRIEF.md`.

Se o usuário posteriormente fornecer reações próprias, atualizar a posição para `USER_CALIBRATED_READER_POSITION` sem refazer a análise da obra. Se fornecer preferência explícita de severidade de nota, ela pode recalibrar a rubrica prospectivamente e, por ordem explícita, retrospectivamente.