# SOURCE_POLICY — Tratamento da Obra-Fonte

## Objetivo

Definir onde a obra original fica e como a IA deve referenciá-la sem confundir armazenamento com capacidade real de leitura.

## Regra de privacidade

Não armazene PDF/EPUB integral protegido por direitos autorais em repositório público.

O repositório `synapselab-ia/clubedolivro` deve ser tornado privado antes de receber obras integrais sem autorização de distribuição.

## GitHub como arquivo x GitHub como fonte legível

Mesmo em repositório privado, um PDF/EPUB pode ficar armazenado no GitHub, mas o conector usado pela IA nem sempre consegue ler binários diretamente como texto.

Portanto, diferencie:

- `STORAGE_SOURCE`: onde o arquivo é arquivado;
- `READABLE_SOURCE`: como a IA efetivamente acessou o conteúdo.

Esses campos devem ser registrados em `BOOK.md`.

## Fluxos permitidos

### Fluxo A — recomendado

1. usuário fornece PDF/EPUB diretamente ao ChatGPT/File Library;
2. GitHub mantém metadados, notas, análises e resultados;
3. opcionalmente, uma cópia do arquivo fica no GitHub privado para arquivo.

### Fluxo B — texto extraído

1. conteúdo da obra é disponibilizado em formato textual legível pela IA;
2. o texto fica em `books/<slug>/source/` em repositório privado;
3. a IA usa esse texto como `READABLE_SOURCE`.

### Fluxo C — somente GitHub binário

Só use se a ferramenta da sessão demonstrar que consegue ler o arquivo integralmente. Não presuma que consegue.

## Pasta de entrada

`books/_inbox/` é o local de entrada para novas obras quando o repositório estiver privado.

Depois da inicialização do livro, a obra pode ser referenciada ou movida conceitualmente para `books/<slug>/source/`.

## Nomes de arquivo

Preferir nomes simples:

- `book.pdf`
- `book.epub`
- `book.txt`

ou nome descritivo sem caracteres desnecessários.

## Integridade da edição

Nunca misture evidências de edições diferentes sem registrar isso.

Se paginação variar, priorize capítulo/seção e registre página apenas como referência auxiliar.
