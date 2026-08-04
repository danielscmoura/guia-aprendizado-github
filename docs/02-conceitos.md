# Capítulo 2: Conceitos Fundamentais do HTML

Agora que você já sabe o que é o HTML e para que ele serve, é hora de entender as engrenagens por trás dessa linguagem. Neste capítulo, vamos explorar a anatomia dos elementos, como funcionam os atributos, a hierarquia das tags e a diferença entre os tipos de exibição na tela.

---

## 1. Tags, Elementos e Conteúdo: Qual é a diferença?

Muitas vezes esses termos são usados como sinônimos, mas eles têm papeis bem definidos na estrutura do HTML:

*   **Tag (Etiqueta):** É o comando delimitado pelos sinais de menor (`<`) e maior (`>`). Exemplo: `<p>` (tag de abertura) e `</p>` (tag de fechamento).
*   **Conteúdo:** É o texto ou a mídia que fica guardado entre a abertura e o fechamento da tag.
*   **Elemento:** É o conjunto completo: **Tag de Abertura + Conteúdo + Tag de Fechamento**.

```html
<!-- Isto é um elemento completo -->
<p>Aprender HTML é o primeiro passo para o desenvolvimento web.</p>
```

---

## 2. Tags Sem Fechamento (Tags Vazia / Void Tags)

Nem todas as tags no HTML precisam de um conteúdo interno ou de uma tag de fechamento correspondente. Elas são chamadas de **tags vazias** ou *self-closing tags*, pois desempenham uma função direta ou inserem um elemento autônomo na página.

Exemplos comuns:
*   `<br>`: Insere uma quebra de linha.
*   `<hr>`: Cria uma linha horizontal divisória.
*   `<img>`: Insere uma imagem na página.
*   `<input>`: Cria um campo de entrada para o usuário digitar.

> **Dica:** No HTML5, você não precisa colocar a barra final nessas tags (escreve-se `<br>` e não `<br />`), embora ambas as formas sejam aceitas pelos navegadores.

---

## 3. Atributos HTML: Personalizando Elementos

Os **atributos** são propriedades usadas para fornecer informações adicionais ou modificar o comportamento de um elemento. Eles sempre ficam dentro da **tag de abertura** e seguem a estrutura de chave e valor: `nome="valor"`.

```html
<a href="https://github.com" target="_blank">Acessar o GitHub</a>
```

Analisando o exemplo acima:
*   `<a>`: Elemento de link (*anchor*).
*   `href="..."`: Atributo que define o destino (endereço URL) do link.
*   `target="_blank"`: Atributo que instrui o navegador a abrir o link em uma nova aba.
*   `Acessar o GitHub`: O texto clicável (conteúdo).

### Atributos Globais Principais
Existem atributos que podem ser usados em praticamente qualquer tag HTML:
*   `id`: Define um identificador único para o elemento no documento (não deve se repetir na mesma página).
*   `class`: Define uma ou mais classes para agrupar elementos (muito usado no CSS e JS).
*   `title`: Exibe uma dica em caixa de texto quando o usuário passa o ponteiro do mouse por cima.
*   `style`: Permite aplicar estilos CSS diretamente na tag (uso recomendado apenas para testes rápidos).

---

## 4. Aninhamento e Hierarquia (Parent/Child)

O HTML funciona como uma estrutura de árvore. Um elemento pode conter outros elementos dentro dele. Quando colocamos um elemento dentro de outro, chamamos esse processo de **aninhamento**.

*   **Pai (Parent):** O elemento que contém outros dentro dele.
*   **Filho (Child):** O elemento contido dentro de outro.

```html
<div>
    <h2>Título da Seção</h2>
    <p>Este parágrafo é um elemento <strong>filho</strong> da div.</p>
</div>
```

### Regras de Ouro do Aninhamento:
1.  **Fechamento correto:** A primeira tag a ser aberta deve ser a última a ser fechada (*Last In, First Out*).
    *   ✅ **Correto:** `<p>Texto <strong>negrito</strong> aqui.</p>`
    *   ❌ **Incorreto:** `<p>Texto <strong>negrito aqui.</p></strong>`
2.  **Indentação:** Sempre alinhe o código interno com espaços ou *Tab*. Isso torna a leitura do seu código muito mais simples para você e para a sua equipe.

---

## 5. Elementos de Bloco (*Block-level*) vs. Elementos de Linha (*Inline*)

Os elementos HTML se comportam de duas maneiras principais no layout da página por padrão:

| Tipo | Comportamento | Exemplos |
| :--- | :--- | :--- |
| **Block-level** (Bloco) | Ocupam **100% da largura** disponível do container. Sempre começam em uma nova linha e empilham uns sobre os outros. | `<div>`, `<h1>`-`<h6>`, `<p>`, `<section>`, `<ul>` |
| **Inline** (Linha) | Ocupam **apenas o espaço necessário** para o seu conteúdo. Permitem que outros elementos fiquem ao lado na mesma linha. | `<span>`, `<a>`, `<strong>`, `<em>`, `<img>` |

---

## 6. Comentários no HTML

Comentários servem para deixar anotações para você ou para outros desenvolvedores no código. O navegador ignora totalmente os comentários e eles **não aparecem na tela** para o usuário.

Sintaxe do comentário:
```html
<!-- Este é um comentário em HTML. Ele não é exibido na página! -->
```

Você também pode usar comentários para desativar temporariamente um trecho de código durante os testes:
```html
<!-- <button>Botão desativado temporariamente</button> -->
```

---

## Resumo do Capítulo

neste capítulo, você aprendeu:
1.  A diferença entre Tag, Conteúdo e Elemento.
2.  O papel dos Atributos (`nome="valor"`) para adicionar propriedades.
3.  A importância da hierarquia, aninhamento correto e indentação.
4.  A diferença crucial entre elementos `block` e `inline`.
5.  Como adicionar comentários para documentar seu código.

No próximo capítulo, vamos colocar a mão na massa para conhecer as **tags essenciais de estruturação de texto e listas**!