# Documentação do Projeto: MovieMind - Jogo de Filmes

Este documento apresenta o funcionamento do programa MovieMind, um jogo de navegador desenvolvido para aplicar conceitos de programação e estruturas de organização de dados através de uma experiência interativa com filmes.

O projeto permite que o usuário tente descobrir um filme secreto utilizando informações cinematográficas como ano, gênero, diretor, país e nota.

---

# 1. Problema que o software resolve

Muitos usuários buscam formas simples de entretenimento que também estimulem o raciocínio e o conhecimento.

O MovieMind resolve esse problema criando um desafio diário de filmes, onde o jogador precisa analisar informações e utilizar tentativas para encontrar a resposta correta.

---

# 2. Solução proposta

O sistema apresenta um filme secreto escolhido automaticamente e permite que o usuário pesquise possíveis respostas.

A cada tentativa, o programa compara as informações do filme escolhido com o filme correto, mostrando quais características estão próximas ou diferentes.

---

# 3. O que este programa faz?

O MovieMind é um jogo onde o usuário precisa descobrir qual é o filme secreto escolhido pelo sistema.

O programa utiliza:

• Banco de Filmes (Lista):
Guarda todos os filmes disponíveis para buscas e escolha do desafio.

• Sistema de Comparação:
Analisa as características do filme escolhido e compara com o filme secreto.

• Escolha Diária:
Define automaticamente um filme diferente utilizando a data atual.

---

# 4. Como funciona por dentro

O arquivo "filmes.json" armazena as informações dos filmes.

Cada filme possui:

- Nome;
- Ano;
- Gênero;
- Diretor;
- País;
- Nota.

O JavaScript realiza a busca, escolhe o filme secreto e compara os dados das tentativas.

---

# 5. Arquitetura do Software

O sistema é dividido em três partes:

## Interface Web

Responsável pela interação com o usuário.

## Motor do Jogo

Desenvolvido em JavaScript e responsável pela lógica do sistema.

## Banco de Dados Local

Arquivo filmes.json responsável pelo armazenamento dos filmes.

---

# 6. Modelo C4 Simplificado

Usuário

↓

Interface Web (HTML/CSS)

↓

Sistema do Jogo (JavaScript)

↓

Banco de Filmes (filmes.json)

---

# 7. Decisões Técnicas

## HTML, CSS e JavaScript

Escolhidos por permitirem uma aplicação simples, leve e executável diretamente no navegador.

## JSON

Escolhido para armazenar os filmes por ser organizado e fácil de atualizar.

## Execução Local

O projeto não depende de servidores ou serviços externos.

---

# 8. Documentação de API

O MovieMind não possui uma API externa.

A comunicação acontece localmente entre o JavaScript e o arquivo filmes.json.

---

# 9. Como executar o programa

1. Baixe todos os arquivos do projeto.

2. Mantenha index.html e filmes.json na mesma pasta.

3. Abra o arquivo index.html no navegador.

---

# 10. Tecnologias utilizadas

• HTML:
Estrutura da aplicação.

• CSS:
Design e identidade visual.

• JavaScript:
Lógica do jogo.

• JSON:
Armazenamento dos filmes.

---

# 11. Direitos de Uso

Este software foi desenvolvido para fins acadêmicos e de estudo.

O projeto pode ser utilizado e modificado para aprendizado, mantendo os créditos dos autores originais.
