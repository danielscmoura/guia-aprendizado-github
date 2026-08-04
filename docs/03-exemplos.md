# Capítulo 3: Exemplos Práticos de HTML

Depois de compreender a teoria e os conceitos fundamentais do HTML, a melhor maneira de fixar o aprendizado é analisando e escrevendo código de verdade. Neste capítulo, reunimos diversos exemplos práticos categorizados por tipo de uso.

---

## 1. Formatação de Texto e Hierarquia de Títulos

Este exemplo demonstra como organizar um artigo simples utilizando diferentes níveis de títulos, parágrafos e destaques de texto.

```html
<h1>O Impacto da Tecnologia no Dia a Dia</h1>

<h2>1. Comunicação Instantânea</h2>
<p>A forma como nos comunicamos mudou drasticamente. Hoje, é possível conversar com pessoas do outro lado do mundo em <strong>tempo real</strong>.</p>

<h2>2. Automação e Produtividade</h2>
<p>Ferramentas modernas permitem automatizar tarefas repetitivas. Isso gera <em>mais tempo livre</em> para focar no que realmente importa.</p>

<hr>

<p><small>Publicado em: <mark>2026</mark> | Fonte: Golldrine Tech</small></p>
```

---

## 2. Listas Ordenadas e Não Ordenadas

Listas são excelentes para organizar passos a passo, requisitos ou coleções de itens.

```html
<!-- Lista Não Ordenada (com marcadores em ponto) -->
<h3>Tecnologias Essenciais para Web Development</h3>
<ul>
    <li>HTML5</li>
    <li>CSS3</li>
    <li>JavaScript</li>
</ul>

<!-- Lista Ordenada (numerada) -->
<h3>Passo a Passo para Criar um Projeto</h3>
<ol>
    <li>Criar a pasta do projeto no computador.</li>
    <li>Abrir a pasta no editor de código (VS Code).</li>
    <li>Criar o arquivo <code>index.html</code>.</li>
    <li>Escrever a estrutura básica e testar no navegador.</li>
</ol>
```

---

## 3. Links e Imagens

Como inserir elementos visuais e criar navegação para outras páginas ou sites externos.

```html
<h3>Galeria e Navegação</h3>

<!-- Imagem com atributo de acessibilidade (alt) -->
<img src="https://via.placeholder.com/400x200" alt="Exemplo de imagem de demonstração" width="400">

<p>Para aprender mais sobre desenvolvimento, visite o <a href="https://developer.mozilla.org/pt-BR/" target="_blank" rel="noopener">MDN Web Docs</a>.</p>
```

---

## 4. Tabelas de Dados

Tabelas devem ser utilizadas para dados estruturados em linhas e colunas (e não para criar o layout do site).

```html
<h3>Tabela de Preços e Planos</h3>

<table border="1">
    <thead>
        <tr>
            <th>Plano</th>
            <th>Recursos</th>
            <th>Preço</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Básico</td>
            <td>Acesso aos guias em PDF</td>
            <td>Grátis</td>
        </tr>
        <tr>
            <td>Pro</td>
            <td>Guias em PDF + Suporte a dúvidas</td>
            <td>R$ 29/mês</td>
        </tr>
    </tbody>
</table>
```

---

## 5. Formulário Simples de Contato

Formulários permitem interagir com o usuário e coletar informações.

```html
<h3>Entre em Contato</h3>

<form action="#" method="POST">
    <!-- Campo de Nome -->
    <label for="nome">Nome Completo:</label><br>
    <input type="text" id="nome" name="nome" placeholder="Digite seu nome" required>
    <br><br>

    <!-- Campo de E-mail -->
    <label for="email">E-mail:</label><br>
    <input type="email" id="email" name="email" placeholder="seu@email.com" required>
    <br><br>

    <!-- Caixa de Mensagem -->
    <label for="mensagem">Sua Mensagem:</label><br>
    <textarea id="mensagem" name="mensagem" rows="4" cols="40" placeholder="Escreva aqui..."></textarea>
    <br><br>

    <!-- Botão de Envio -->
    <button type="submit">Enviar Mensagem</button>
</form>
```

---

## 6. Exemplo Integrado: Página Completa

Abaixo está um documento HTML5 completo juntando todos os elementos vistos acima em uma única estrutura funcional.

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Primeiro Site Completo</title>
</head>
<body>

    <header>
        <h1>Bem-vindo ao Guia de HTML</h1>
        <p>Aprenda a criar páginas web do zero!</p>
    </header>

    <main>
        <section>
            <h2>Sobre o Projeto</h2>
            <p>Este é um exemplo de página completa construída com <strong>tags semânticas</strong> do HTML5.</p>
        </section>

        <section>
            <h2>O que você vai aprender:</h2>
            <ul>
                <li>Estruturar textos e parágrafos</li>
                <li>Criar formulários de captura</li>
                <li>Organizar dados com tabelas</li>
            </ul>
        </section>

        <section>
            <h2>Inscreva-se na Newsletter</h2>
            <form>
                <input type="email" placeholder="Digite seu e-mail" required>
                <button type="submit">Cadastrar</button>
            </form>
        </section>
    </main>

    <footer>
        <hr>
        <p>&copy; 2026 - Criado por Daniel Moura (Golldrine Tech)</p>
    </footer>

</body>
</html>
```

---

## Próximo Passo

Copie qualquer um dos códigos acima, salve em um arquivo com final `.html` na sua máquina e abra-o com dois cliques no seu navegador de preferência para ver o resultado em tempo real!