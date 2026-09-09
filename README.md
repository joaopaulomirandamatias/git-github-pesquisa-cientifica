# Git e GitHub para pesquisadores: passo a passo (MirandasTech)

Manual em formato de slides (50) para versionar o projeto de pesquisa na pós-graduação: o que é o Git e por que usar (o que a evidência e os guias dizem), Git × GitHub × GitLab, o que entra e o que fica fora do repositório (dados pessoais e LGPD, material licenciado, segredos, arquivos grandes e os limites do GitHub), instalar e configurar; o Git no dia a dia com o terminal aberto (init, status, add, commit, log, .gitignore, branch, diff, merge, tag por marco, conflitos, desfazer com segurança); o GitHub passo a passo sem login (planos, criar repositório e «Olá, Mundo», remoto e push, a página de um repositório real, commits e Actions, issues e pull requests, GitHub Desktop e VS Code, CLI e Codespaces, Pages, Git LFS, Overleaf e OSF); publicar com README, licença, `CITATION.cff` e «Cite this repository», releases e DOI pelo Zenodo, GitLab como alternativa; os scripts `checar_repo.py`, `citacao_cff.py` e `salvar_versao.sh`; erros comuns, checklist, glossário com popovers e referências. Capturas reais e datadas (09/09/2026) de páginas públicas e uma sessão real de terminal; nenhuma captura exigiu login e nenhum repositório foi criado na conta do autor para a demonstração.

**Manual on-line:** https://git.mirandastech.com.br/ · **PDF:** https://git.mirandastech.com.br/manual.pdf

Manuais irmãos: **LaTeX com Overleaf e abnTeX2** — https://latex.mirandastech.com.br/ · **Busca em bases científicas** — https://busca.mirandastech.com.br/ · **Revisão sistemática com PRISMA 2020** — https://prisma.mirandastech.com.br/ · **Zotero** — https://zotero.mirandastech.com.br/ · **Metodologia** — https://metodologia.mirandastech.com.br/ · **Gemini Notebook** — https://notebook.mirandastech.com.br/ · **Uso de IA na pesquisa** — https://manual.mirandastech.com.br/ · **Plugin Pesquisa (Claude e Codex)** — https://plugin.mirandastech.com.br/ · Hub: https://www.mirandastech.com.br/pesquisa

| Pasta | O que há |
|---|---|
| `manual/` | deck HTML autônomo, PDF, fonte do artefato e `fatos_verificados.md` (todas as fontes, versões e comandos conferidos em 09/09/2026) |
| `site/` | o que o servidor serve (`index.html`, `manual.pdf`) |
| `capturas/` | 40 capturas reais, 09/09/2026 (36 telas públicas do GitHub, Git, Zenodo, Overleaf, GitLab, VS Code e guias; 4 figuras de terminal com saídas reais) |
| `scripts/checar_repo.py` | auditoria antes de publicar: arquivos acima de 50/100 MiB, segredos, dados pessoais, pastas de dados, README/LICENSE/CITATION.cff/.gitignore, remoto |
| `scripts/salvar_versao.sh` | commit com resumo do que entra, recusa arquivos acima de 100 MiB, tag anotada por marco |
| `scripts/citacao_cff.py` | gera o `CITATION.cff` 1.2.0 e mostra a entrada BibTeX e a referência ABNT |
| `scripts/gerar_deck.py` | regenera HTML e PDF a partir do fonte |
| `skills/git-github-pesquisadores/` | skill do agente (cópia sincronizada do plugin Pesquisa MirandasTech) |
| `Dockerfile` · `Caddyfile` · `railway.json` | deploy estático (Caddy) |
| `.github/workflows/verificar.yml` | CI: integridade do deck e capturas referenciadas |

## Os manuais juntos
Este manual cobre o **controle de versão** do projeto: do primeiro commit ao DOI. O projeto nasce com Git pelo plugin **Pesquisa MirandasTech** (`pesquisa-mirandastech`, `iniciar_projeto.py`), o texto vem do manual de LaTeX (`latex-overleaf-abntex2-pesquisa-cientifica`) e a biblioteca do Zotero (`zotero-pesquisa-cientifica`). No plugin, a skill `git-github-pesquisadores` audita e explica; o aluno cria o repositório, a release e o DOI, e nada de dado pessoal ou licenciado entra no Git.

## Como citar
MATIAS, J. P. M. *Git e GitHub para pesquisadores: passo a passo.* MirandasTech, v1.0, set. 2026. CC BY 4.0.

## Declaração de uso de IA
Escrito com assistência de IA (Claude, Anthropic) na estruturação, redação, automação das capturas e execução dos scripts e dos comandos. Versões, nomes de botões, planos e preços, limites e referências conferidos nas fontes oficiais e em comandos reais em 09/09/2026 (lista em `manual/fatos_verificados.md`); nenhuma captura foi feita com login. O autor responde integralmente pelo conteúdo. GitHub, Git, GitLab, Zenodo, OSF, Overleaf, Microsoft e os demais serviços citados são marcas e projetos de terceiros; este manual não tem vínculo com eles.
