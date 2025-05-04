# Problema de Coloração de Grafos - Algoritmos e Estruturas de Dados

Este projeto implementa duas abordagens diferentes para resolver o problema de coloração de grafos, um problema clássico em Ciência da Computação. O problema consiste em atribuir cores aos vértices de um grafo de forma que nenhum par de vértices adjacentes compartilhe a mesma cor, utilizando o menor número possível de cores.

## Estrutura do Projeto

O projeto é composto por três arquivos principais:

1. `main.py`: Arquivo principal que contém a lógica de execução e visualização do problema
2. `coloracao_heuristica.py`: Implementa uma solução heurística usando o algoritmo DSATUR
3. `coloracao_baseline.py`: Implementa uma solução de força bruta para encontrar a solução ótima

## Funcionalidades

### Algoritmo Heurístico (DSATUR)

- Implementa o algoritmo DSATUR, uma heurística eficiente para coloração de grafos
- Seleciona vértices baseado em sua saturação (número de cores diferentes usadas nos vizinhos)
- Em caso de empate, escolhe o vértice com maior grau
- Visualiza o grafo colorido usando a biblioteca NetworkX

### Algoritmo Baseline (Força Bruta)

- Implementa uma solução de força bruta para encontrar a solução ótima
- Gera todas as possíveis combinações de cores
- Verifica cada combinação para encontrar a que usa o menor número de cores
- Também visualiza o grafo colorido

## Requisitos

Para executar o projeto, são necessárias as seguintes bibliotecas Python:

- numpy
- pandas
- matplotlib
- networkx

## Como Usar

1. Execute o arquivo `main.py`
2. O programa gera um grafo aleatório com o número de vértices especificado
3. Aplica ambos os algoritmos (heurístico e baseline)
4. Exibe os resultados, incluindo:
   - Número cromático do grafo
   - Tempo de execução
   - Visualização gráfica do grafo colorido

## Exemplo de Saída

O programa exibe:

- Lista de elementos químicos (vértices)
- Lista de cores atribuídas
- Número cromático do grafo
- Tempo de execução em milissegundos
- Distribuição dos elementos por container (cor)

## Observações

- O algoritmo baseline (força bruta) é computacionalmente intensivo e pode ser lento para grafos grandes
- O algoritmo heurístico (DSATUR) é mais eficiente, mas pode não encontrar a solução ótima
- O projeto inclui visualização gráfica do grafo colorido usando diferentes cores para cada container
