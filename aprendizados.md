# Registro de Aprendizados e Reflexão Final

Este documento registra a reflexão sobre o fluxo de trabalho adotado durante a criação do **Guia de Fundamentos de HTML**, destacando os aprendizados práticos com controle de versão, colaboração no GitHub e organização do projeto.

---

## 1. Controle de Versão com Git

A prática continuada de comandos do Git permitiu consolidar conceitos essenciais para o dia a dia de desenvolvimento:

*   **Trabalho com Branches:** Em vez de realizar alterações diretamente na branch `main`, utilizar ramificações temáticas (`feature/*` ou `feat/*`) garante que o código principal permaneça estável e funcional enquanto novos capítulos ou arquivos estão sendo desenvolvidos.
*   **Resolução de Conflitos de Merge:** O manuseio direto de conflitos (identificando e limpando marcadores como `<<<<<<< HEAD`, `=======` e `>>>>>>>`) reforçou a importância de analisar as diferenças entre trechos de código e escolher a versão final unificada mais coerente.
*   **Sincronização entre Local e Remoto:** A resolução de falhas de sincronização ensinou a importância do comando `git fetch` para atualizar as referências do repositório remoto e de comandos como `git reset --hard` para alinhar o ambiente local quando o histórico diverge.

---

## 2. Fluxo de Pull Requests e Colaboração no GitHub

O processo de envio e integração de código no GitHub seguiu o padrão de boas práticas de mercado:

*   **Rastreabilidade:** Cada alteração foi enviada para o repositório remoto via `git push`, permitindo a abertura de **Pull Requests (PRs)** específicos.
*   **Transparência e Revisão:** O link do Pull Request atua como ponto central de auditoria, onde é possível visualizar o histórico de *commits*, inspecionar o *diff* de cada arquivo modificado e discutir melhorias antes da integração final com a branch `main`.
*   **Merge Seguro:** Realizar o *merge* do PR diretamente pela interface da plataforma assegura um registro claro da fusão do código no repositório.

---

## 3. Modularização da Documentação em Markdown

A estrutura do projeto foi planejada para garantir escalabilidade e fácil manutenção:

*   **Separação por Capítulos:** A divisão sequencial dos arquivos (`01-introducao.md`, `02-conceitos.md`, `03-exemplos.md` e `04-referencias.md`) facilita a leitura do estudante e a navegação por tópicos específicos.
*   **Padronização de Licença:** A avaliação das opções de licença (como MIT ou Creative Commons) evidenciou como a escolha dos direitos de uso é fundamental ao publicar projetos e guias em repositórios abertos.

---

## 4. Conclusão

A aplicação do fluxo completo de Git e GitHub — desde o planejamento dos arquivos até o envio, resolução de conflitos e fusão via Pull Request — provou que o domínio dessas ferramentas é tão indispensável quanto a escrita da própria linguagem HTML. Esse padrão de fluxo de trabalho estabelece uma base sólida para a construção e manutenção de projetos mais complexos no futuro.