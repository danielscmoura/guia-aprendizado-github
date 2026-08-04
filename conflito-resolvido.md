# Resolução de Conflito de Merge

## 1. Como o conflito foi gerado
O conflito foi gerado de forma intencional alterando o mesmo trecho/linha ("Linha editada na branch") em dois pontos distintos do histórico:
1. A linha foi criada e inserida na branch de *feature*.
2. Em seguida, na branch `main`, a mesma linha foi editada/modificada de maneira divergente antes de realizar a fusão.
Ao tentar executar o `git merge`, o Git identificou que a mesma linha havia recebido alterações concorrentes e interrompeu o processo para evitar perda de dados.

## 2. Como foi identificado
O terminal emitiu um alerta informando sobre a colisão de dados:
```text
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.
```
Ao abrir o arquivo `README.md` no editor de código, o Git delimitou o conflito utilizando os marcadores padrão:
* `<<<<<<< HEAD` (versão atual presente na `main`)
* `=======` (separador)
* `>>>>>>> feature/...` (versão vinda da branch de trabalho)

## 3. Como foi resolvido
1. O arquivo `README.md` foi aberto no editor de código.
2. Analisou-se o trecho controverso contendo a "Linha editada na branch" sob ambas as perspectivas.
3. Os marcadores de conflito (`<<<<<<<`, `=======`, `>>>>>>>`) foram removidos manualmente.
4. O texto final foi ajustado para manter a versão correta e unificada desejada.
5. A resolução foi consolidada no repositório executando:
   ```bash
   git add README.md
   git commit -m "Resolve conflito de merge no README"
   ```