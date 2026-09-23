# Documentação do Projeto: MovieMind - Jogo de Filmes

Este documento explica de forma simples e direta o funcionamento do
programa MovieMind, um jogo de navegador desenvolvido para testar o
conhecimento dos usuários sobre filmes.

O objetivo do programa é criar uma experiência de entretenimento onde o
jogador tenta descobrir um filme secreto através de dicas e comparações
de informações cinematográficas.

## 1. O que este programa faz?

O MovieMind é um jogo onde o usuário precisa descobrir qual é o filme
secreto escolhido pelo sistema.

Para isso, o jogador digita nomes de filmes e recebe comparações entre o
filme escolhido e o filme correto.

O programa utiliza conceitos básicos de programação para organizar essas
informações:

• O Banco de Filmes (Lista): Guarda todos os filmes disponíveis para que
o sistema possa realizar buscas e escolher o desafio do dia.

• Sistema de Comparação: Analisa as características do filme escolhido
pelo jogador e compara com o filme secreto.

• Escolha Diária: Define automaticamente um filme diferente como desafio
utilizando a data atual do computador.

## 2. Como as coisas funcionam por dentro

Para organizar os dados, o programa utiliza algumas lógicas importantes:

• Lista de Filmes:

Exemplo prático: Pense em uma biblioteca com vários filmes cadastrados.
Cada filme possui informações como nome, ano, gênero, diretor, país e
nota.

No programa: O arquivo "filmes.json" funciona como uma base de dados
simples, armazenando todas essas informações para serem utilizadas
durante o jogo.

• Sistema de Comparação:

Exemplo prático: Quando alguém tenta adivinhar um filme, é possível
comparar características para descobrir se está próximo ou distante da
resposta correta.

No programa: O sistema verifica informações como ano, gênero, diretor,
país e nota, mostrando quais dados estão corretos ou diferentes.

• Escolha do Filme do Dia:

Exemplo prático: Assim como desafios diários encontrados em jogos
online, o jogador recebe um novo desafio a cada dia.

No programa: A data atual é utilizada para escolher automaticamente qual
filme será o desafio.

## 3. Como usar o programa no computador

Para executar e testar o projeto:

• O que você precisa: Um navegador atualizado (Google Chrome, Microsoft
Edge, Firefox ou similar).

• Como executar:

-   Baixe todos os arquivos do projeto.

-   Mantenha o arquivo "filmes.json" na mesma pasta do "index.html".

-   Abra o arquivo "index.html" no navegador.

• O que vai acontecer:

O programa irá carregar a lista de filmes, escolher automaticamente o
filme secreto do dia e permitir que o usuário realize tentativas até
encontrar a resposta.

## 4. Tecnologias utilizadas

O projeto foi desenvolvido utilizando:

• HTML: Responsável pela estrutura da página.

• CSS: Responsável pela aparência e identidade visual do jogo.

• JavaScript: Responsável pela lógica do funcionamento do sistema.

• JSON: Utilizado para armazenar as informações dos filmes.

## 5. Sobre os Direitos de Uso (Licença)

Este software foi desenvolvido para fins acadêmicos e de estudo.

O projeto pode ser utilizado, modificado e compartilhado para
aprendizado, mantendo os créditos dos autores originais.
