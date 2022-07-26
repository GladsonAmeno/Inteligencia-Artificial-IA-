# Projeto 0a: Degrees

Escreva um programa que determine quantos “graus de separação” existem entre dois atores.

```
$ python degrees.py large
Carregando dados...
Dados Carregados.
Nome: Emma Watson
Nome: Jennifer Lawrence
3 graus de separação.
1: Emma Watson and Brendan Gleeson starred in Harry Potter and the Order of the Phoenix
2: Brendan Gleeson and Michael Fassbender starred in Trespass Against Us
3: Michael Fassbender and Jennifer Lawrence starred in X-Men: First Class
```

## Background

De acordo com o jogo [Six Degrees of Kevin Bacon](https://en.wikipedia.org/wiki/Six_Degrees_of_Kevin_Bacon), qualquer pessoa na indústria cinematográfica de Hollywood pode se conectar a Kevin Bacon em seis etapas,
onde cada passo consiste em encontrar um filme que dois atores protagonizem.

Neste problema, estamos interessados em encontrar o caminho mais curto entre quaisquer dois atores escolhendo uma sequência de filmes que os conecte.
Por exemplo, o caminho mais curto entre Jennifer Lawrence e Tom Hanks é 2: Jennifer Lawrence está ligada a Kevin Bacon por ambos estrelando
em “X-Men: Primeira Classe”, e Kevin Bacon está conectado a Tom Hanks por ambos estrelando “Apollo 13”.

Podemos enquadrar isso como um problema de busca: nossos estados são pessoas. Nossas ações são filmes, que nos levam de um ator a outro (é verdade
que um filme pode nos levar a vários atores diferentes, mas tudo bem para esse problema). Nosso estado inicial e estado objetivo são definidos
pelas duas pessoas que estamos tentando conectar. Ao usar a busca em largura, podemos encontrar o caminho mais curto de um ator para outro.

## Especificação

Conclua a implementação da função shortest_path de forma que ela retorne o caminho mais curto da pessoa com a origem do id para a pessoa com o id de destino.

- Supondo que haja um caminho da origem para o destino, sua função deve retornar uma lista, onde cada item da lista é o próximo par (id_do_filme, id_pessoa) no caminho da origem para o destino. Cada par deve ser uma tupla de dois ints.
    - Por exemplo, se o valor de retorno de shortest_path fosse [(1, 2), (3, 4)], isso significaria que a fonte estrelou o filme 1 com a pessoa 2, a pessoa 2 estrelou o filme 3 com a pessoa 4 e pessoa 4 é o alvo.
- Se houver vários caminhos de comprimento mínimo da origem ao destino, sua função poderá retornar qualquer um deles.
- Se não houver caminho possível entre dois atores, sua função deve retornar Nenhum.
- Você pode chamar a função neighbors_for_person, que aceita o id de uma pessoa como entrada e retorna um conjunto de pares (movie_id, person_id) para todas as pessoas que estrelaram um filme com uma determinada pessoa.

Você não deve modificar nada no arquivo além da função shortest_path, embora possa escrever funções adicionais e/ou importar outros módulos de biblioteca padrão do Python.

## Reconhecimentos

Informações cortesia de [IMDb](https://www.imdb.com/). Usado com permissão.
