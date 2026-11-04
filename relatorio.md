# Relatório Técnico - Moviez

## Objetivo
Aplicar conceitos de programação e estruturas de dados em um quiz interativo de filmes, com perguntas geradas automaticamente a partir de um catálogo.

## Estruturas utilizadas
- Lista (array) de objetos de filmes, carregada de um arquivo JSON
- Conjuntos (Set) para garantir alternativas sem repetição
- Lista de perguntas, onde cada pergunta é um objeto com texto, opções e resposta correta
- Vetor de histórico de acertos e erros, usado na tela de resultado

## Algoritmos
- **Gerador pseudoaleatório com semente:** a data do dia define o sorteio, então o quiz é o mesmo para todos no mesmo dia.
- **Embaralhamento (Fisher-Yates):** usado para sortear filmes e misturar as alternativas.
- **Geração de alternativas erradas:** anos e notas próximos ao valor correto; diretores e gêneros escolhidos de outros filmes do catálogo, sem repetir a resposta certa.
- **Comparação de atributos:** na pergunta de maior nota, o código percorre quatro filmes e encontra o maior valor.

## Funcionamento
O sistema carrega o filmes.json e monta 10 perguntas de múltipla escolha (diretor, ano, gênero e nota). O usuário escolhe uma alternativa por pergunta e recebe feedback imediato, com a resposta certa destacada. Ao final, o sistema mostra a nota (acertos de 10) e o histórico de respostas.

## Resultados e limitações
- O quiz funciona sem servidor ou API externa, apenas com HTML, CSS, JavaScript e JSON.
- Cada filme tem um único gênero, o que pode gerar dúvidas em filmes de gêneros mistos.
- Os pôsteres são opcionais e dependem de uma chave gratuita da API do TMDB.

## Melhorias futuras
- Salvar o resultado do dia (localStorage) e permitir compartilhamento da pontuação.
- Adicionar novos campos ao JSON (elenco, sinopse) para novos tipos de pergunta.
- Criar ranking, tempo por pergunta e níveis de dificuldade.
