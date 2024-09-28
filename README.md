# ArvoreDOM

## Descrição do Projeto##
Este projeto é uma demonstração simples de como manipular a árvore DOM utilizando JavaScript. O objetivo é modificar o conteúdo de um elemento específico na página e adicionar novos elementos dinâmicamente.

## Estrutura do Projeto 
O projeto consiste em dois arquivos principais:

DOM.js: Contém a função JavaScript que realiza as operações de manipulação do DOM.
index.html: Arquivo HTML que estrutura a página e inclui o script JavaScript.

## Detalhes Técnicos

*** Arquivo 1: DOM.js - 
Função divEdit:
Objetivo: Modificar o conteúdo do elemento com ID header e adicionar um novo parágrafo.
Processo:
Busca o elemento: Utiliza document.getElementById("header") para obter o elemento desejado.
Guarda o conteúdo atual: Armazena o HTML existente na variável conteudo.
Reescreve o conteúdo: Altera o HTML do elemento, adicionando tags <strong> ao conteúdo atual.
Criação de novo elemento:
Cria um novo elemento <p> com document.createElement('p').
Define um atributo title para o parágrafo com paragrafo.setAttribute('title', 'Novo parágrafo').
Cria um nó de texto com document.createTextNode() e o adiciona ao novo parágrafo.
Inserção na árvore DOM: O novo parágrafo é anexado ao elemento header com header.appendChild(paragrafo).

*** Arquivo 2: index.html - 
Estrutura básica: Utiliza XHTML 1.0 Strict para garantir conformidade com padrões web.
Elementos:
Um <div> com ID header que contém texto inicial.
Um botão de entrada (<input type="button">) que, ao ser clicado, executa a função divEdit().

### Funcionamento: 
Quando o botão "Altera árvore DOM" é clicado, a função divEdit() é chamada.
A função manipula o conteúdo do elemento header, adicionando formatação e inserindo um novo parágrafo.
O novo parágrafo aparece abaixo do texto original, mostrando como a árvore DOM foi alterada dinamicamente.


### Conclusão
Esse projeto é uma boa introdução às manipulações do DOM, demonstrando a adição e modificação de elementos na página web. Ele serve como base para aplicações mais complexas onde interações dinâmicas são necessárias.
