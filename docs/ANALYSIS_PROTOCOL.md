# ANALYSIS_PROTOCOL — Análise de Cada Parte

Este protocolo é obrigatório para cada bloco da obra.

## Objetivo

Produzir notas suficientemente compactas para reutilização por outra IA, mas suficientemente ricas para reconstruir fatos, arcos, temas e evidências sem reler o bloco inteiro.

## Antes de analisar

1. Confirme o escopo exato da parte.
2. Leia `BOOK.md` e `STATUS.md`.
3. Leia as análises anteriores necessárias para continuidade.
4. Não antecipe acontecimentos ainda não alcançados, salvo quando marcados explicitamente como contexto externo.

## Estrutura mínima

### 1. Escopo

Registrar capítulos, páginas ou outra unidade estável.

### 2. Resumo factual

Explicar de modo compacto o que ocorre no bloco, preservando relações causais importantes.

### 3. Eventos relevantes

Lista dos acontecimentos que provavelmente terão impacto posterior.

### 4. Personagens

Para cada personagem relevante nesta parte:
- estado/situação;
- ações;
- motivações aparentes;
- conflitos;
- mudanças;
- relações alteradas;
- informação nova.

### 5. Arcos e progressão

Registrar o que começou, avançou, regrediu ou foi encerrado nesta parte.

### 6. Temas

Não basta nomear temas. Para cada tema observado, registrar:
- como aparece;
- quem/qual evento o manifesta;
- evidência de suporte;
- se é recorrente ou apenas possível.

### 7. Símbolos, motivos e padrões

Registrar objetos, imagens, espaços, frases, situações ou estruturas que aparentem recorrência ou função simbólica.

Não elevar coincidência isolada a símbolo sem marcar como hipótese.

### 8. Passagens-chave

Para cada passagem importante:
- localização;
- paráfrase ou citação curta quando necessária;
- contexto;
- por que importa;
- tema/arco associado.

### 9. Afirmações interpretativas

Classificar a confiança:
- `HIGH`: múltiplas evidências ou suporte textual forte;
- `MEDIUM`: leitura plausível com suporte parcial;
- `LOW/HYPOTHESIS`: possibilidade ainda a testar.

### 10. Conexões com partes anteriores

Registrar continuidade, contraste, repetição, consequência ou revisão de hipóteses anteriores.

### 11. Contradições ou revisões

Se uma hipótese anterior enfraqueceu, registre explicitamente em vez de apagá-la retroativamente.

### 12. Questões em aberto

Perguntas que a análise futura precisa observar.

### 13. Itens para revisitar

Elementos que devem ser conferidos na consolidação/auditoria.

## Densidade esperada

As notas devem priorizar informação de alto valor analítico. Evite:
- recontar cada microevento;
- adjetivos vagos;
- elogios genéricos;
- inferências psicológicas sem base;
- repetir a mesma conclusão em seções diferentes.

## Regra de rastreabilidade

Sempre que uma interpretação for importante para a obra inteira, associe-a a pelo menos uma evidência localizável.

## Regra de continuidade

Ao concluir uma parte:

1. crie/atualize `analysis/NN.md`;
2. marque a parte como concluída no `STATUS.md`;
3. registre a próxima parte como `NEXT_ACTION`, ou avance para consolidação quando todas estiverem concluídas.
