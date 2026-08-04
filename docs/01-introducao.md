# Capítulo 1: Introdução ao HTML

Bem-vindo ao primeiro passo da sua jornada no desenvolvimento web! Antes de começarmos a escrever linhas de código, é fundamental entendermos o que é o HTML e qual o seu papel na internet.

## O que é HTML?

HTML é a sigla para **HyperText Markup Language** (Linguagem de Marcação de Hipertexto). 

É importante esclarecer logo de cara: **HTML não é uma linguagem de programação**. Ele não possui lógica, não toma decisões, não faz cálculos e não usa variáveis. O HTML é uma **linguagem de marcação**. 

Isso significa que ele é usado para "marcar" ou estruturar o conteúdo de uma página web, dizendo ao navegador (como o Chrome, Edge ou Firefox) o que é cada elemento. É ele quem define: "isto é um título", "isto é um parágrafo", "isto é uma imagem" ou "isto é um link".

## A Metáfora da Construção

Para entender como o HTML se encaixa no desenvolvimento de um site, pense na construção de uma casa:

*   **HTML (A Estrutura):** São os tijolos e as vigas. É a base de tudo. Sem ele, a página não existe. Ele sustenta os textos, imagens e formulários.
*   **CSS (O Acabamento):** É a pintura, a decoração e o design. O CSS adiciona cores, define fontes, ajusta tamanhos e posiciona os elementos na tela para deixar tudo agradável visualmente.
*   **JavaScript (A Eletricidade e Encanamento):** É o que dá vida à casa. O JavaScript adiciona interatividade, permitindo que botões executem ações, animações aconteçam e dados sejam enviados.

## Como o HTML funciona?

A base do HTML são as **Tags** (etiquetas). As tags geralmente funcionam em pares: uma tag de abertura e uma tag de fechamento, envolvendo o conteúdo que queremos estruturar.

Exemplo prático:
```html
<p>Este é um parágrafo de exemplo.</p>
```
*   `<p>` é a tag de abertura (o "p" vem de *paragraph*).
*   `Este é um parágrafo de exemplo.` é o conteúdo visível.
*   `</p>` é a tag de fechamento (note a presença da barra inclinada `/`).

## A Estrutura Básica de um Documento HTML

Todo arquivo HTML (salvo com a extensão `.html`) precisa de uma estrutura mínima para ser lido corretamente pelos navegadores. Ela se parece com isto:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Primeira Página</title>
</head>
<body>
    <h1>Olá, Mundo!</h1>
    <p>Esta é a estrutura básica para começar a criar para a web.</p>
</body>
</html>
```

No próximo capítulo, vamos destrinchar cada uma dessas linhas para entender exatamente o que elas fazem, além de prepararmos o seu ambiente para você começar a programar na prática!