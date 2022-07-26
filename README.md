# Meu trabalho na introdução à IA com Python do CS50´s

https://cs50.harvard.edu/ai/

Este curso explora os conceitos e algoritmos na base da inteligência artificial moderna, mergulhando no
ideias que dão origem a tecnologias como mecanismos de jogo, reconhecimento de caligrafia e tradução automática.
Por meio de projetos práticos, os alunos ganham exposição à teoria por trás dos algoritmos de busca em grafos, classificação,
otimização, aprendizado por reforço e outros tópicos em inteligência artificial e aprendizado de máquina à medida que
incorporá-los em seus próprios programas Python. Ao final do curso, os alunos emergem com experiência em bibliotecas para
aprendizado de máquina, bem como o conhecimento dos princípios de inteligência artificial que lhes permitem projetar
sistemas próprios.
 
Certificado:
Em curso...

## Palestra 0: Search

### Conceitos
- **Agent**: entity that perceives its environment and acts upon that environment.
  - **Agente**: Entidade que percebe seu ambiente e age sobre esse ambiente.
- **State**: a configuration of the agent and its environment.
  - **Estado**: Uma configuração do agente e seu ambiente.
- **Actions**: choices that can be made in a state.
  - **Ações**: Escolhas que podem ser feitas em um estado.
- **Transition model**: a description of what state results from performing any applicable action in any state.
  - **Modelo de Transição**: Uma descrição de qual estado resulta da execução de qualquer ação aplicável em qualquer estado.
- **Path cost**: numerical cost associated with a given path.
  - **Custo de Caminho**: Custo numérico associado a um determinado caminho.
- **Evaluation function**: function that estimates the expected utility of the game from a given state.
  - **Função de Avaliação**: Função que estima a utilidade esperada do jogo a partir de um determinado estado.

### Algoritmos
- **DFS** (depth first search): search algorithm that always expands the deepest node in the frontier.
- **BFS** (breath first search): search algorithm that always expands the shallowest node in the frontier.
- **Greedy best-first search**: search algorithm that expands the node that is closest to the goal, as estimated by an
 heuristic function _h(n)_.
- **A\* search**: search algorithm that expands node with lowest value of the "cost to reach node" plus the "estimated
 goal
 cost".
- **Minimax**: adversarial search algorithm.

### Projetos
- [Degrees](https://github.com/GladsonAmeno/Inteligencia-Artificial-IA-/tree/main/degrees)
- [Tic-Tac-Toe] - Em desenvolvimento...
