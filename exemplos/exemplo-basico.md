# Exemplo Básico de HTML

Este é um modelo mínimo e funcional de uma página HTML5. Você pode copiar o código abaixo, salvar em um arquivo chamado `index.html` no seu computador e abri-lo com dois cliques em qualquer navegador.

---

## Código HTML

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Página Básica</title>
</head>
<body>

    <header>
        <h1>Minha Primeira Página Web</h1>
    </header>

    <main>
        <section>
            <h2>Sobre Este Exemplo</h2>
            <p>Este arquivo demonstra a estrutura mínima necessária para construir um documento HTML5 válido, acessível e bem formatado.</p>
        </section>

        <section>
            <h2>Lista de Primeiros Passos</h2>
            <ul>
                <li>Criar o arquivo <code>index.html</code></li>
                <li>Colar esta estrutura básica</li>
                <li>Abrir no navegador para visualizar o resultado</li>
            </ul>
        </section>
    </main>

    <footer>
        <hr>
        <p>&copy; 2026 - Guia de Fundamentos de HTML</p>
    </footer>

</body>
</html>
```

---

## Explicação das Tags Utilizadas

* **`<!DOCTYPE html>`:** Declara ao navegador que o documento utiliza a versão mais recente do HTML (HTML5).
* **`<html lang="pt-BR">`:** Elemento raiz do documento, definindo o idioma principal como português do Brasil (essencial para leitores de tela e acessibilidade).
* **`<head>`:** Guarda as configurações e metadados da página, como a codificação de caracteres (`UTF-8`) e o título da aba.
* **`<body>`:** Contém todo o conteúdo visível para o usuário final (cabeçalho, seções de texto, listas e rodapé).