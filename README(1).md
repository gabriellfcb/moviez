# Documentação do Projeto: Moviez - Quiz de Filmes

Este documento apresenta o funcionamento do programa Moviez, um quiz de navegador desenvolvido para aplicar conceitos de programação e estruturas de organização de dados através de uma experiência interativa com filmes.

O projeto propõe um quiz diário de 10 perguntas de múltipla escolha sobre diretor, ano, gênero e nota de filmes.

---

# 1. Problema que o software resolve

Muitos usuários buscam formas simples de entretenimento que também estimulem o raciocínio e o conhecimento.

O Moviez resolve esse problema criando um quiz diário de cinema, com perguntas curtas e feedback imediato, que incentiva o jogador a voltar todos os dias.

---

# 2. Solução proposta

O sistema gera automaticamente 10 perguntas a partir do catálogo de filmes. Cada pergunta tem 4 alternativas, e o jogador escolhe uma delas.

A cada resposta, o programa mostra se o jogador acertou ou errou, indica a alternativa correta e atualiza o placar. No final, exibe a nota e o histórico de acertos.

---

# 3. O que este programa faz?

O Moviez é um quiz onde o usuário responde perguntas sobre filmes escolhidas pelo sistema.

O programa utiliza:

• Banco de Filmes (Lista):
Guarda todos os filmes disponíveis, usados para criar perguntas e alternativas.

• Gerador de Perguntas:
Monta as 10 perguntas do quiz e sorteia alternativas erradas a partir do próprio catálogo.

• Escolha Diária:
Define automaticamente o quiz do dia utilizando a data atual como semente do sorteio, garantindo as mesmas perguntas para todos os jogadores no mesmo dia.

• Sistema de Validação:
Compara a alternativa escolhida com a resposta correta e calcula a pontuação.

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

O JavaScript carrega o catálogo, gera as perguntas do dia, valida as respostas e controla o placar.

## Tipos de pergunta

| Tipo | Exemplo | Quantidade |
|------|---------|-----------|
| Diretor | Quem dirigiu «filme»? | 3 |
| Ano | Em que ano foi lançado «filme»? | 3 |
| Gênero | Qual é o gênero de «filme»? | 2 |
| Nota | Qual é a nota de «filme»? | 1 |
| Maior nota | Qual destes 4 filmes tem a maior nota? | 1 |

As alternativas erradas são escolhidas assim: anos próximos ao correto, notas próximas na mesma faixa, e diretores e gêneros sorteados de outros filmes do catálogo.

---

# 5. Arquitetura do Software

O sistema é dividido em três partes:

## Interface Web

Responsável pela interação com o usuário: pergunta, alternativas, feedback verde/vermelho, barra de progresso e tela de resultado.

## Motor do Quiz

Desenvolvido em JavaScript e responsável pela lógica do sistema: geração das perguntas, sorteio com semente, validação e pontuação.

## Banco de Dados Local

Arquivo filmes.json responsável pelo armazenamento dos filmes.

---

# 6. Modelo C4 Simplificado

Usuário

↓

Interface Web (HTML/CSS)

↓

Motor do Quiz (JavaScript)

↓

Banco de Filmes (filmes.json)

---

# 7. Decisões Técnicas

## HTML, CSS e JavaScript

Escolhidos por permitirem uma aplicação simples, leve e executável diretamente no navegador.

## JSON

Escolhido para armazenar os filmes por ser organizado e fácil de atualizar. Ao adicionar um filme, ele passa a ser usado nas perguntas automaticamente.

## Sorteio com semente

A data do dia (ano, mês e dia) alimenta um gerador de números pseudoaleatórios. Assim, o quiz muda todos os dias, mas é o mesmo para todos no mesmo dia, sem precisar de servidor.

## Execução Local

O projeto não depende de servidores ou serviços externos para funcionar.

---

# 8. Documentação de API

O Moviez não depende de API externa para funcionar.

A comunicação principal acontece localmente entre o JavaScript e o arquivo filmes.json.

Opcionalmente, o projeto pode exibir pôsteres usando a API gratuita do TMDB. Para isso, basta colar a chave da API na constante `TMDB_KEY` do arquivo index.html. Sem a chave, o quiz funciona normalmente, apenas sem imagens.

---

# 9. Como executar o programa

1. Baixe todos os arquivos do projeto.

2. Mantenha index.html e filmes.json na mesma pasta.

3. Abra o projeto por um servidor local, pois os navegadores bloqueiam a leitura do filmes.json quando o index.html é aberto direto do arquivo. Opções:
   - Extensão **Live Server** no VS Code (botão "Go Live");
   - Terminal: `python -m http.server` na pasta do projeto e acessar http://localhost:8000;
   - Publicar no GitHub Pages.

4. (Opcional) Cole sua chave do TMDB em `TMDB_KEY` para exibir os pôsteres.

---

# 10. Tecnologias utilizadas

• HTML:
Estrutura da aplicação.

• CSS:
Design e identidade visual.

• JavaScript:
Lógica do quiz.

• JSON:
Armazenamento dos filmes.

• TMDB (opcional):
Pôsteres dos filmes.

---

# 11. Direitos de Uso

Este software foi desenvolvido para fins acadêmicos e de estudo.

O projeto pode ser utilizado e modificado para aprendizado, mantendo os créditos dos autores originais.
