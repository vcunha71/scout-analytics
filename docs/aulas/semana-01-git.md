# Semana 1: Organizar a casa (Git e versionamento)

> Data: 10/11/2026 · Repositório: https://github.com/vcunha71/scout-analytics

## 1. O que construímos

| # | O que | Onde |
|---|---|---|
| 1 | Repositório Git na pasta `project_vitorscout` | PC |
| 2 | Estrutura profissional: `src/`, `sql/`, `notebooks/`, `docs/`, `data/` | PC + GitHub |
| 3 | `.gitignore` protegendo os dados do Wyscout e as pastas do Drive | PC + GitHub |
| 4 | README de portfólio com 3 perguntas de scout | GitHub |
| 5 | Licença MIT + documentação da fonte de dados | GitHub |
| 6 | Repositório público no ar | github.com/vcunha71/scout-analytics |
| 7 | Backup da pasta inteira, com os dados | Google Drive |

## 2. Histórico de commits

1. `9dc72ef chore:` estrutura inicial
2. `3cd2c71 docs:` perguntas no README (feito por mim)
3. `d0ea18e chore:` ignorar pastas temporárias do Google Drive (feito por mim)

## 3. Conceitos

1. **Git:** histórico de mudanças com autor, data e motivo.
2. **GitHub:** cópia oficial na nuvem + vitrine do portfólio.
3. **Fluxo (analogia do jogo):**
   - `git add` = escalação (escolhe o que entra)
   - `git commit` = súmula assinada (foto salva no PC, com mensagem)
   - `git push` = enviar para a federação (vai para o GitHub)
4. **Commit não roda nada.** Ele só salva uma foto dos arquivos. Rodar é `python script.py`.
5. **`.gitignore`:** lista do que é invisível para o Git. Protege dados licenciados e senhas.
6. **Git ≠ backup.** GitHub guarda código e histórico; o Drive guarda os dados. Se o HD morrer, preciso dos dois.
7. **E-mail noreply:** liga os commits ao perfil sem expor o e-mail pessoal.
8. **Conventional Commits:** `feat:` novidade, `fix:` correção, `docs:` documentação, `chore:` manutenção.

## 4. Colinha de comandos

```
git status          # o que mudou? (só olha)
git add arquivo     # escalar um arquivo
git commit -m "..." # salvar a foto com mensagem
git push            # enviar para o GitHub
git log --oneline   # ver o histórico
```

Evitar `git add .` sem ter certeza do que vai entrar.

## 5. Alternativas que existiam

1. **Só OneDrive/Drive com versões:** guarda versões, mas sem mensagem, sem diferença linha a linha e sem revisão. Serve para backup, não para trabalho em equipe.
2. **Subir os dados para o GitHub:** mais simples, mas fere a licença do Wyscout e incha o repositório. Em empresa, seria vazar dado de cliente.

## 6. Como as empresas usam

1. **Pull Request:** ninguém altera a `main` direto; um colega revisa antes.
2. **CI/CD:** cada commit dispara testes automáticos (semana 6, dbt).
3. **PBIP/TMDL (semana 9):** o modelo do Power BI vira texto, e o Git mostra qual medida DAX mudou, linha por linha.

## 7. Lições do dia

1. O GitHub **não** tem os dados, só o código.
2. Apareceu um problema real (pasta temporária do Drive) e foi resolvido com `.gitignore`.
3. Mudanças diferentes vão em commits separados (`docs:` e `chore:`), o que facilita a revisão.

## Resumo em 5 linhas

1. Git = histórico de mudanças; GitHub = cópia oficial na nuvem.
2. Fluxo: editar → `git add` → `git commit` → `git push`.
3. `.gitignore` protege o que não pode sair do PC.
4. Git é para o código, backup é para os dados: um não substitui o outro.
5. Nas empresas, o Git é a base de revisão (PR), testes e deploy, inclusive no Power BI com PBIP.
