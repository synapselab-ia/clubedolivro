# AUDIT_PROTOCOL — Auditoria Adversarial

A auditoria ocorre depois da consolidação e antes da análise crítica final.

## Objetivo

Tentar refutar, corrigir ou enfraquecer as conclusões produzidas durante a leitura antes que elas apareçam nos materiais finais.

## Procedimento

### 1. Integridade factual

Verifique:
- cronologia;
- nomes e identidades;
- relações entre personagens;
- causalidade de eventos;
- quem disse/fez o quê;
- sequência de revelações;
- diferenças entre fato narrado e relato de personagem.

### 2. Cobertura

Pergunte:
- algum personagem ou arco importante foi subanalisado?
- há parte da obra quase ausente da síntese?
- algum tema relevante apareceu repetidamente sem consolidação?
- o começo e o fim da obra foram tratados com o mesmo rigor?

### 3. Teste de interpretações

Para cada interpretação central:

1. Qual é a evidência mais forte a favor?
2. Qual é a melhor evidência contra?
3. Existe explicação alternativa mais simples?
4. A interpretação depende de conhecimento externo não sinalizado?
5. O texto realmente exige essa leitura ou apenas a permite?

Classifique o resultado:
- `SUPPORTED`;
- `SUPPORTED_WITH_CAVEATS`;
- `UNCERTAIN`;
- `REJECTED`.

### 4. Teste de símbolos e temas

Remova ou rebaixe elementos tratados como símbolo/tema quando:
- aparecem isoladamente;
- dependem apenas de associação subjetiva;
- não produzem efeito estrutural relevante;
- contradizem evidências mais fortes.

### 5. Contradições internas

Compare todas as análises parciais e arquivos de síntese em busca de:
- hipóteses incompatíveis;
- mudança de interpretação não registrada;
- avaliações de personagem inconsistentes;
- duplicidades que mascaram falta de evidência.

### 6. Linguagem inflada

Marque como fraca qualquer formulação que pareça sofisticada mas não seja operacionalizável ou sustentada.

Exemplos a evitar:
- “a obra explora a complexidade da condição humana” sem especificação;
- “o autor desconstrói paradigmas sociais” sem mostrar onde e como.

### 7. Lacunas

Crie uma seção `NEEDS_SOURCE_RECHECK` caso alguma conclusão relevante exija retorno à fonte original.

Não invente preenchimento para uma lacuna.

## Saída obrigatória — `synthesis/AUDIT.md`

O arquivo deve conter:

- `FACTUAL_CORRECTIONS`;
- `INTERPRETATIONS_CONFIRMED`;
- `INTERPRETATIONS_DOWNGRADED`;
- `INTERPRETATIONS_REJECTED`;
- `MISSING_OR_UNDERWEIGHTED_ELEMENTS`;
- `NEEDS_SOURCE_RECHECK`;
- `FINAL_CONFIDENCE_NOTES`.

## Regra de passagem

Só avance para síntese crítica quando nenhuma correção factual importante estiver pendente sem registro explícito.
