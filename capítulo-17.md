# CAPÍTULO 17 — ALGORITMOS DE ORDENAÇÃO

## Como Organizar Dados de Forma Eficiente

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que é ordenação.
* Compreender por que ordenar dados é importante.
* Conhecer os principais algoritmos de ordenação.
* Implementar Bubble Sort.
* Implementar Selection Sort.
* Implementar Insertion Sort.
* Entender Merge Sort.
* Entender Quick Sort.
* Comparar desempenho entre algoritmos.
* Aplicar ordenação em sistemas reais.

---

# Introdução

Imagine uma lista de alunos:

```text
Lucas
Ana
Pedro
Carlos
Maria
```

Encontrar um nome específico pode ser difícil.

Agora observe:

```text
Ana
Carlos
Lucas
Maria
Pedro
```

Tudo está organizado.

A busca se torna muito mais fácil.

---

# O Que é Ordenação?

Definição:

> Ordenação é o processo de organizar elementos seguindo uma determinada regra.

Exemplos:

* Ordem alfabética.
* Ordem crescente.
* Ordem decrescente.
* Data mais recente.
* Maior nota.
* Menor preço.

---

# Por Que Ordenar?

Muitos algoritmos funcionam melhor com dados ordenados.

Exemplo:

A Busca Binária estudada no capítulo anterior exige:

```text
Lista ordenada
```

Sem ordenação:

```text
40 10 80 20 50
```

Busca binária não funciona corretamente.

---

# Aplicações Reais

Empresas utilizam ordenação diariamente.

Exemplos:

### Netflix

Ordenar filmes por popularidade.

### Spotify

Ordenar músicas por reproduções.

### Amazon

Ordenar produtos por preço.

### Bancos

Ordenar transações por data.

---

# Exemplo Inicial

Lista:

```text
5 3 8 1 4
```

Ordenada:

```text
1 3 4 5 8
```

---

# Bubble Sort

É o algoritmo de ordenação mais famoso entre iniciantes.

Também é conhecido como:

```text
Ordenação por Bolha
```

---

# Como Funciona?

Compara elementos vizinhos.

Se estiverem fora de ordem:

```text
Troca
```

---

Exemplo

Lista:

```text
5 3 8 1
```

Primeira comparação:

```text
5 > 3
```

Troca.

Resultado:

```text
3 5 8 1
```

---

Segunda comparação:

```text
5 < 8
```

Nada acontece.

---

Terceira comparação:

```text
8 > 1
```

Troca.

Resultado:

```text
3 5 1 8
```

---

# Implementação do Bubble Sort

```python
numeros = [5,3,8,1,4]

n = len(numeros)

for i in range(n):

    for j in range(0, n-i-1):

        if numeros[j] > numeros[j+1]:

            numeros[j], numeros[j+1] = numeros[j+1], numeros[j]

print(numeros)
```

---

Resultado:

```text
[1, 3, 4, 5, 8]
```

---

# Visualização do Processo

```text
5 3 8 1 4

↓

3 5 8 1 4

↓

3 5 1 8 4

↓

3 5 1 4 8

↓

1 3 4 5 8
```

---

# Complexidade do Bubble Sort

O(n^2)

Significa:

```text
Quanto mais elementos

↓

Muito mais trabalho
```

---

# Vantagens

* Fácil de entender.
* Fácil de implementar.

---

# Desvantagens

* Muito lento.
* Não utilizado em sistemas grandes.

---

# Selection Sort

Outro algoritmo clássico.

---

# Como Funciona?

Procura o menor elemento.

Depois coloca na posição correta.

---

Exemplo

Lista:

```text
5 3 8 1 4
```

Menor valor:

```text
1
```

Troca com o primeiro.

Resultado:

```text
1 3 8 5 4
```

---

# Implementação

```python
numeros = [5,3,8,1,4]

for i in range(len(numeros)):

    menor = i

    for j in range(i+1, len(numeros)):

        if numeros[j] < numeros[menor]:

            menor = j

    numeros[i], numeros[menor] = numeros[menor], numeros[i]

print(numeros)
```

---

Resultado:

```text
[1,3,4,5,8]
```

---

# Complexidade

O(n^2)

Semelhante ao Bubble Sort.

---

# Insertion Sort

Inspirado na forma como organizamos cartas de baralho.

---

# Funcionamento

Pegamos um elemento.

Inserimos na posição correta.

---

Exemplo

```text
5 3 8 1
```

Pegamos:

```text
3
```

Inserimos antes do 5.

Resultado:

```text
3 5 8 1
```

---

# Implementação

```python
numeros = [5,3,8,1,4]

for i in range(1, len(numeros)):

    chave = numeros[i]

    j = i - 1

    while j >= 0 and numeros[j] > chave:

        numeros[j+1] = numeros[j]

        j -= 1

    numeros[j+1] = chave

print(numeros)
```

---

Resultado:

```text
[1,3,4,5,8]
```

---

# Quando o Insertion Sort é Bom?

Quando existem poucos dados.

Ou quando os dados já estão quase ordenados.

---

# Complexidade

O(n^2)

---

# Comparação dos Três

| Algoritmo      | Fácil | Rápido |
| -------------- | ----- | ------ |
| Bubble Sort    | Sim   | Não    |
| Selection Sort | Sim   | Não    |
| Insertion Sort | Sim   | Médio  |

---

# Surge um Problema

Imagine:

```text
1.000.000 registros
```

Os algoritmos anteriores ficam lentos.

Precisamos de algo melhor.

---

# Merge Sort

Um dos algoritmos mais importantes da computação.

---

# Estratégia

Divide para conquistar.

---

Funcionamento:

```text
Lista grande

↓

Divide em partes menores

↓

Ordena cada parte

↓

Junta tudo
```

---

Exemplo

```text
8 3 5 1
```

Divide:

```text
8 3

5 1
```

---

Ordena:

```text
3 8

1 5
```

---

Junta:

```text
1 3 5 8
```

---

# Complexidade

O(n\log n)

Muito melhor.

---

# Vantagens

* Muito rápido.
* Estável.
* Amplamente utilizado.

---

# Desvantagens

* Consome memória extra.

---

# Quick Sort

Considerado um dos algoritmos mais importantes da história da computação.

---

Desenvolvido por:

Tony Hoare

---

# Funcionamento

Escolhe um pivô.

---

Exemplo

Lista:

```text
5 3 8 1 4
```

Pivô:

```text
5
```

---

Menores:

```text
3 1 4
```

---

Maiores:

```text
8
```

---

Resultado:

```text
3 1 4 | 5 | 8
```

---

Repete o processo.

---

# Complexidade Média

O(n\log n)

---

# Complexidade Pior Caso

O(n^2)

---

Mesmo assim, na prática é extremamente eficiente.

---

# Comparação Geral

| Algoritmo      | Complexidade |
| -------------- | ------------ |
| Bubble Sort    | O(n²)        |
| Selection Sort | O(n²)        |
| Insertion Sort | O(n²)        |
| Merge Sort     | O(n log n)   |
| Quick Sort     | O(n log n)   |

---

# Qual Utilizar?

Poucos dados:

```text
Insertion Sort
```

---

Aprendizado:

```text
Bubble Sort
```

---

Grandes volumes:

```text
Merge Sort
Quick Sort
```

---

# Ordenação em Python

Python já possui ordenação pronta.

---

Exemplo:

```python
numeros = [5,3,8,1,4]

numeros.sort()

print(numeros)
```

---

Resultado:

```text
[1,3,4,5,8]
```

---

Também:

```python
sorted(numeros)
```

---

# Ordenação Decrescente

```python
numeros.sort(reverse=True)
```

---

Resultado:

```text
[8,5,4,3,1]
```

---

# Ordenando Textos

```python
nomes = [

    "Lucas",

    "Ana",

    "Carlos"

]

nomes.sort()
```

---

Resultado:

```text
Ana
Carlos
Lucas
```

---

# Aplicação Real

Sistema Escolar

Ordenar alunos por nota.

---

# Aplicação Real

E-commerce

Ordenar produtos por:

* Menor preço.
* Maior preço.
* Mais vendidos.

---

# Aplicação Real

Redes Sociais

Ordenar:

* Comentários.
* Curtidas.
* Seguidores.

---

# Erros Mais Comuns

## Erro 1

Tentar usar busca binária sem ordenar primeiro.

---

## Erro 2

Escolher algoritmo inadequado.

---

## Erro 3

Ignorar complexidade.

---

# Exercícios Resolvidos

## Exercício 1

Ordenar lista.

```python
numeros = [7,3,9,1]

numeros.sort()

print(numeros)
```

---

## Exercício 2

Ordenar decrescente.

```python
numeros.sort(reverse=True)
```

---

# Exercícios

1. Implementar Bubble Sort.
2. Implementar Selection Sort.
3. Implementar Insertion Sort.
4. Ordenar nomes.
5. Ordenar notas.
6. Ordenar lista crescente.
7. Ordenar lista decrescente.
8. Comparar algoritmos.
9. Medir tempo de execução.
10. Ordenar produtos.

---

# Desafio

Crie um sistema que:

1. Cadastre 20 alunos.
2. Armazene nome e nota.
3. Ordene pela maior nota.
4. Mostre um ranking.
5. Exiba o Top 5.

---

# Curiosidade

Os algoritmos de ordenação estão entre os mais estudados da computação. Grandes empresas como Google, Amazon, Microsoft e Meta utilizam versões altamente otimizadas desses algoritmos para processar bilhões de registros diariamente.

---

# Resumo do Capítulo

Você aprendeu:

* O que é ordenação.
* Bubble Sort.
* Selection Sort.
* Insertion Sort.
* Merge Sort.
* Quick Sort.
* Complexidade dos algoritmos.
* Aplicações reais.
* Uso em sistemas modernos.
