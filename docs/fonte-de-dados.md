# Fonte de dados

## O que é

Exportações de estatísticas por equipe ("Team Stats") do Brasileirão Série A 2026, um arquivo Excel por clube (20 clubes).

## Formato bruto

- 1 aba por arquivo (`TeamStats`).
- 2 linhas por partida: a equipe e o adversário.
- ~109 colunas: golos, xG, remates, passes, posse, PPDA, duelos, recuperações etc.
- Cabeçalho em 3 linhas, com colunas compostas (ex.: "Remates / à baliza" ocupa 2 colunas: total e certos).
- Termos em português de Portugal (golos, remates, cantos).

## Regras de uso

- Os arquivos brutos **não** são versionados: `data/` está no `.gitignore`.
- Cada pessoa que clonar o repositório precisa colocar os próprios arquivos em `data/`.
- Só código, documentação e resultados agregados sobem para o GitHub.

## Próximo passo

Semana 3: script Python que lê os 20 arquivos, trata o cabeçalho e carrega tudo num banco DuckDB.
