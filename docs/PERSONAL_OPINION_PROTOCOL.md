# PERSONAL_OPINION_PROTOCOL — Construção da Posição de Leitor

## Objetivo

Transformar a análise auditada da obra em uma **posição de leitor específica, plausível e defensável para uso do usuário**, sem exigir que ele tenha realizado a leitura integral por conta própria.

O modo padrão é:

`CONSTRUCTED_READER_POSITION`

O usuário pode fornecer reações pessoais, mas isso é opcional. Quando existirem, elas prevalecem sobre preferências geradas pela IA.

## Princípio central

A IA deve construir uma posição que uma pessoa bem informada consiga sustentar em conversa porque conhece:

- fatos importantes do enredo;
- arcos dos personagens;
- escolhas formais;
- temas centrais;
- ambiguidades;
- pontos fortes e limitações reais da obra.

A posição não deve ser um resumo neutro. Precisa fazer escolhas avaliativas.

## Inputs obrigatórios

- `synthesis/AUDIT.md`;
- `synthesis/CRITICAL_ANALYSIS.md`;
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

## Procedimento

1. extrair da síntese 3–5 méritos fortes da obra;
2. identificar 1–3 limitações ou reservas defensáveis;
3. escolher uma avaliação geral coerente com esse balanço;
4. definir uma nota aproximada compatível com a avaliação;
5. selecionar personagem, relação ou elemento mais marcante;
6. avaliar ritmo e estilo de forma específica;
7. formular posição sobre o final;
8. escolher ao menos uma interpretação com a qual a posição construída concorda fortemente;
9. escolher ao menos uma nuance, crítica ou discordância para evitar opinião artificialmente perfeita;
10. preparar argumentos curtos que possam ser usados em conversa;
11. registrar contra-argumentos plausíveis e respostas defensáveis;
12. salvar em `synthesis/READER_POSITION.md`.

## Estrutura mínima de `READER_POSITION.md`

- `MODE`: `CONSTRUCTED_READER_POSITION` ou `USER_CALIBRATED_READER_POSITION`;
- avaliação geral;
- nota;
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

## Proibições

Não:

- inventar fatos da obra;
- criar citações inexistentes;
- afirmar que o usuário leu uma passagem específica;
- inventar experiências sensoriais ou cronológicas de leitura, como “quando cheguei nesse capítulo fiquei...”;
- transformar hipótese rejeitada pela auditoria em opinião factual;
- produzir uma posição tão genérica que pudesse servir para qualquer livro.

## Critério de conclusão

`PERSONALIZE` está concluído quando existe um `synthesis/READER_POSITION.md` coerente com a auditoria e suficientemente específico para alimentar `final/MY_OPINION.md` e `final/BOOK_CLUB_BRIEF.md`.

Se o usuário posteriormente fornecer reações próprias, atualizar a posição para `USER_CALIBRATED_READER_POSITION` sem refazer a análise da obra.