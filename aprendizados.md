# Registro de Aprendizados e Reflexão Final

Este documento registra a reflexão sobre o fluxo de trabalho adotado durante a criação do **Guia de Fundamentos de HTML**, destacando os aprendizados práticos com controle de versão, colaboração no GitHub, resolução de conflitos e organização do projeto.

---

## 1. Controle de Versão com Git

A prática continuada de comandos do Git permitiu consolidar conceitos essenciais para o dia a dia de desenvolvimento:

*   **Trabalho com Branches:** Em vez de realizar alterações diretamente na branch `main`, utilizar ramificações temáticas (`feature/*`) garantiu que o código principal permanecesse estável enquanto novos arquivos e documentos eram desenvolvidos.
*   **Resolução de Conflitos de Merge:** O manuseio direto de divergências — como a edição concorrente da mesma linha do `README.md` entre a branch principal e a de feature — exigiu identificar os marcadores de conflito, limpá-los manualmente e consolidar a versão correta.
*   **Sincronização entre Local e Remoto:** A gestão do histórico de commits e a integração contínua alinharam perfeitamente o ambiente local com o repositório remoto.

---

## 2. Fluxo de Pull Requests e Colaboração no GitHub

O processo de envio e integração de código seguiu rigorosamente as boas práticas de mercado:

*   **Rastreabilidade:** Cada alteração foi enviada para o repositório remoto via `git push`, permitindo a abertura de **Pull Requests (PRs)** específicos para cada nova entrega (como arquivos de licença, exemplos e documentações).
*   **Merge Seguro:** Realizar o *merge* dos PRs diretamente pela interface da plataforma garantiu o registro histórico de cada adição ao projeto.

---

## 3. Evidência do Histórico de Commits (`git log`)

Abaixo está o registro gráfico extraído diretamente do terminal (`git log --oneline --graph --all`), evidenciando o fluxo de criação das branches de *feature*, os commits específicos e os *merges* via Pull Request integrados à branch `main`:

```text
*   24da08f (HEAD -> main, origin/main, origin/HEAD) Merge pull request #9 from danielscmoura/feature/conflito-resolvido
|\  
| * 512f8d4 (origin/feature/conflito-resolvido, feature/conflito-resolvido) feat: conflito-resolvido.md adicionado
|/  
*   c4b785d fix:Resolve conflito no READ.me
|\  
| * 1912dba (feature/gerar-conflito) docs: recria o conflito sem fastfoward
* | f00b3c2 docs: edita mesma linha de gerar-conflito na main
|/  
* ce68369 Atualiza linha de conflito
* 45927e3 docs: adiciona linha de conflito controlado
*   65c1e89 Merge pull request #8 from danielscmoura/feature/exemplo-basico
|\  
| * 574e2ff (origin/feature/exemplo-basico, feature/exemplo-basico) feat: exemplo-basico.md criado
|/  
*   50822e4 Merge pull request #7 from danielscmoura/feature/aprendizados
|\  
| * 5333909 (origin/feature/aprendizados, feature/aprendizados) feat: aprendizados.md criado
|/  
*   d69b125 Merge pull request #6 from danielscmoura/feature/LICENSE
|\  
| * f4e42a2 (origin/feature/LICENSE, feature/LICENSE) feat: LICENSE criado
|/  
*   76ba905 Merge pull request #5 from danielscmoura/feature/04-referencias
|\  
| * a0345eb (origin/feature/04-referencias, feature/04-referencias) feat: 04-referencias.md criado
|/  
```

---

## 4. Conclusão

A aplicação do fluxo completo de Git e GitHub — desde o planejamento modular dos arquivos em Markdown até a simulação e resolução controlada de um conflito de merge — consolidou competências fundamentais de engenharia de software e controle de versão.