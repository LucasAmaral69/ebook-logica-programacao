# CAPÍTULO 16 — BUSCA LINEAR E BUSCA BINÁRIA

## Como os Computadores Encontram Informações

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o conceito de busca.
* Compreender como computadores localizam dados.
* Implementar Busca Linear.
* Implementar Busca Binária.
* Comparar desempenho entre algoritmos.
* Entender complexidade temporal.
* Saber quando utilizar cada método.
* Aplicar buscas em sistemas reais.

---

# Introdução

Imagine que você possui uma lista telefônica com:

```text
1.000.000 de nomes
```

E precisa encontrar:

```text
Lucas do Amaral Ramos
```

Como faria?

Existem várias estratégias.

Algumas são lentas.

Outras são extremamente rápidas.

A área da computação que estuda isso é chamada de:

```text
Algoritmos de Busca
```

---

# O Que é uma Busca?

Definição:

> Busca é o processo de localizar um elemento dentro de uma coleção de dados.

---

Exemplos:

* Procurar um contato.
* Encontrar um produto.
* Buscar um usuário.
* Encontrar uma mensagem.
* Localizar um arquivo.

---

# Por Que a Busca é Importante?

Praticamente todo sistema realiza buscas.

Exemplos:

### Google

Busca páginas.

### YouTube

Busca vídeos.

### Netflix

Busca filmes.

### Instagram

Busca usuários.

### Banco

Busca contas.

---

# Cenário Simples

Lista:

```text
[10, 20, 30, 40, 50]
```

Procurando:

```text
40
```

Como encontrar?

---

# Busca Linear

Também chamada de:

```text
Busca Sequencial
```

---

Funcionamento:

```text
Começa no início

↓

Verifica elemento

↓

Encontrou?

↓

Sim → Finaliza

Não → Continua
```

---

# Exemplo Visual

Lista:

```text
[10, 20, 30, 40, 50]
```

Buscando:

```text
40
```

---

Passo 1

```text
10 ≠ 40
```

---

Passo 2

```text
20 ≠ 40
```

---

Passo 3

```text
30 ≠ 40
```

---

Passo 4

```text
40 = 40
```

Encontrado.

---

# Implementação em Python

```python
numeros = [10,20,30,40,50]

procurado = 40

for numero in numeros:

    if numero == procurado:

        print("Encontrado")
```

---

Resultado:

```text
Encontrado
```

---

# Retornando a Posição

```python
numeros = [10,20,30,40,50]

procurado = 40

for i in range(len(numeros)):

    if numeros[i] == procurado:

        print(i)
```

---

Resultado:

```text
3
```

---

# Vantagens da Busca Linear

* Fácil implementação.
* Funciona em qualquer lista.
* Não exige ordenação.

---

# Desvantagens

* Lenta em listas grandes.
* Verifica muitos elementos.

---

# Complexidade da Busca Linear

Se existirem:

```text
10 elementos
```

Pode verificar até:

```text
10 elementos
```

---

Se existirem:

```text
1.000.000 elementos
```

Pode verificar até:

```text
1.000.000 elementos
```

---

Complexidade:

```text
O(n)
```

---

# Entendendo O(n)

Significa:

```text
Quanto mais elementos

↓

Mais tempo
```

---

# Problema da Busca Linear

Imagine:

```text
100 milhões de registros
```

Buscar elemento por elemento torna-se caro.

Precisamos de algo melhor.

---

# Busca Binária

A Busca Binária é um dos algoritmos mais importantes da computação.

---

Mas possui uma regra:

```text
A lista deve estar ordenada.
```

---

Exemplo

Lista:

```text
[10,20,30,40,50,60,70]
```

---

Buscando:

```text
60
```

---

# Como Funciona?

A Busca Binária divide a lista ao meio.

---

Visualmente:

```text
10 20 30 40 50 60 70

           ↑

          Meio
```

---

Meio:

```text
40
```

---

Pergunta:

```text
60 > 40 ?
```

Resposta:

```text
Sim
```

---

Então descartamos metade da lista.

---

Restante:

```text
50 60 70
```

---

Novo meio:

```text
60
```

---

Encontrado.

---

# O Poder da Busca Binária

Lista:

```text
1.000.000 elementos
```

---

Busca Linear:

```text
Até 1.000.000 comparações
```

---

Busca Binária:

```text
Aproximadamente 20 comparações
```

---

Diferença gigantesca.

---

# Implementação em Python

```python
numeros = [10,20,30,40,50,60,70]

inicio = 0

fim = len(numeros) - 1

procurado = 60

while inicio <= fim:

    meio = (inicio + fim) // 2

    if numeros[meio] == procurado:

        print("Encontrado")

        break

    elif numeros[meio] < procurado:

        inicio = meio + 1

    else:

        fim = meio - 1
```

---

# Explicação do Algoritmo

Variáveis:

```text
inicio

fim

meio
```

---

Calculamos:

```python
meio = (inicio + fim) // 2
```

---

Depois verificamos:

```text
É igual?
```

---

Se não:

```text
Menor?

Maior?
```

---

E descartamos metade da lista.

---

# Comparação Visual

Busca Linear:

```text
1
2
3
4
5
6
7
8
9
10
```

Percorre um por um.

---

Busca Binária:

```text
1 2 3 4 5 6 7 8 9 10

↓

5

↓

8

↓

9
```

Muito mais rápida.

---

# Complexidade da Busca Binária

Complexidade:

```text
O(log n)
```

---

Significado:

Cada passo reduz a quantidade de dados pela metade.

---

Exemplo

1.024 elementos.

```text
1024

↓

512

↓

256

↓

128

↓

64

↓

32

↓

16

↓

8

↓

4

↓

2

↓

1
```

---

Apenas:

```text
10 passos
```

---

# Comparação de Desempenho

| Elementos | Linear    | Binária |
| --------- | --------- | ------- |
| 100       | 100       | 7       |
| 1.000     | 1.000     | 10      |
| 10.000    | 10.000    | 14      |
| 1.000.000 | 1.000.000 | 20      |

---

# Quando Utilizar Busca Linear?

Use quando:

* Lista pequena.
* Dados não ordenados.
* Simplicidade é prioridade.

---

# Quando Utilizar Busca Binária?

Use quando:

* Lista ordenada.
* Muitos registros.
* Alto desempenho necessário.

---

# Aplicação Real

Agenda Telefônica.

---

Lista ordenada:

```text
Ana

Carlos

João

Lucas

Maria
```

---

Você abre aproximadamente no meio.

Faz exatamente uma busca binária.

---

# Aplicação Real

Dicionários.

---

Ao procurar uma palavra:

```text
Computador
```

Você não começa na página 1.

Abre próximo da letra C.

---

Busca Binária.

---

# Aplicação Real

Banco de Dados

Sistemas modernos utilizam:

* Índices
* Árvores B
* Árvores B+

Todos baseados em conceitos semelhantes à busca binária.

---

# Aplicação Real

Google

O Google utiliza estruturas muito mais avançadas.

Mas os princípios fundamentais de busca continuam presentes.

---

# Erros Mais Comuns

## Erro 1

Usar busca binária em lista desordenada.

---

Exemplo:

```text
40 10 80 20 50
```

Não funciona.

---

## Erro 2

Calcular o meio incorretamente.

---

Correto:

```python
meio = (inicio + fim) // 2
```

---

## Erro 3

Atualizar limites errados.

---

Correto:

```python
inicio = meio + 1

fim = meio - 1
```

---

# Exercícios Resolvidos

## Exercício 1

Encontrar número 15.

```python
numeros = [5,10,15,20]

for numero in numeros:

    if numero == 15:

        print("Encontrado")
```

---

## Exercício 2

Retornar posição.

```python
for i in range(len(numeros)):

    if numeros[i] == 15:

        print(i)
```

---

# Exercícios

1. Implementar busca linear.
2. Retornar posição.
3. Procurar nome em lista.
4. Procurar nota em vetor.
5. Contar comparações.
6. Implementar busca binária.
7. Encontrar posição.
8. Comparar tempos.
9. Testar listas grandes.
10. Criar função de busca.

---

# Desafio

Crie um programa que:

1. Gere uma lista com 100.000 números.
2. Procure um valor usando Busca Linear.
3. Procure o mesmo valor usando Busca Binária.
4. Conte quantas comparações cada algoritmo realizou.
5. Compare os resultados.

---

# Curiosidade

A busca binária é considerada um dos algoritmos mais elegantes da computação porque consegue localizar elementos em enormes conjuntos de dados utilizando pouquíssimas comparações.

---

# Resumo do Capítulo

Você aprendeu:

* O que é busca.
* Busca Linear.
* Busca Binária.
* Complexidade O(n).
* Complexidade O(log n).
* Comparação de desempenho.
* Aplicações reais.
* Casos de uso.
