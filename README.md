# Scout Analytics ⚽📊

Projeto de dados de ponta a ponta sobre o **Brasileirão Série A 2026**: da planilha bruta ao agente de IA que responde perguntas de scout em português.

> *End-to-end football analytics project: raw match data → SQL warehouse → dbt → Power BI → AI agent.*

## Por que este projeto existe

Clubes, analistas e torcedores tomam decisões com dados espalhados em planilhas. Este repositório mostra, passo a passo, como transformar esses dados em um produto analítico confiável: modelado, testado, versionado e pronto para IA.

## Perguntas que este projeto vai responder

1. Quais times marcam mais (ou menos) gols do que o xG indica?
2. Quem pressiona mais alto (menor PPDA) e isso vira recuperações e vitórias?
3. Quais times dependem mais de contra-ataques e quais de ataques posicionais?
## Status

🟢 **Semana 1 de 24: estrutura do repositório**

| Etapa | Entrega | Status |
|---|---|---|
| Base | Repositório, estrutura e documentação | ✅ Em andamento |
| Dados e SQL | Ingestão em Python + DuckDB, SQL avançado, modelo estrela | ⏳ Planejado |
| Qualidade | Modelos e testes com dbt | ⏳ Planejado |
| Power BI | Modelo semântico em PBIP/TMDL, medidas DAX, relatório de scout | ⏳ Planejado |
| Nuvem | Lakehouse e pipeline no Microsoft Fabric | ⏳ Planejado |
| IA | Servidor MCP e agente de scout com avaliação de acertos | ⏳ Planejado |

## Dados

- **Fonte:** estatísticas por equipe e por partida do Brasileirão Série A 2026 (20 equipes).
- **Os dados brutos não estão no repositório.** São licenciados e ficam apenas na máquina local (a pasta `data/` é ignorada pelo Git). Detalhes em [`docs/fonte-de-dados.md`](docs/fonte-de-dados.md).

## Estrutura

```
scout-analytics/
├── data/        # dados brutos locais (fora do Git)
├── src/         # código Python (ingestão e transformação)
├── sql/         # consultas e modelos SQL
├── notebooks/   # exploração e análises
└── docs/        # documentação do projeto
```

## Stack planejada

Python · pandas · DuckDB · SQL · dbt · Power BI (PBIP/TMDL, DAX) · Microsoft Fabric · Claude API · MCP

## Autor

**Vitor Cunha**: consultor sênior de BI (Power BI, SQL/PL-SQL, Python, Oracle Analytics Cloud) com MBA em Análise de Desempenho pela CBF Academy. Criador do Vitor Scout.

- GitHub: [@vcunha71](https://github.com/vcunha71)
- Instagram: [@ovitorscout](https://instagram.com/ovitorscout)
