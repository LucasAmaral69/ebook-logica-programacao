# CAPÍTULO 13 — VETORES E ARRAYS

## Como Armazenar Grandes Quantidades de Dados de Forma Eficiente

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que são vetores e arrays.
* Compreender por que eles existem.
* Armazenar múltiplos valores em uma única variável.
* Utilizar índices.
* Percorrer vetores utilizando loops.
* Realizar buscas em vetores.
* Inserir e alterar valores.
* Resolver problemas reais utilizando coleções de dados.
* Compreender a base para estruturas de dados mais avançadas.

---

# Introdução

Até agora trabalhamos com variáveis individuais.

Exemplo:

```python
nome1 = "Lucas"
nome2 = "Maria"
nome3 = "João"
nome4 = "Pedro"
nome5 = "Ana"
```

Agora imagine uma escola com:

```text
500 alunos
```

Ou uma loja com:

```text
10.000 produtos
```

Criar uma variável para cada item seria impossível.

Foi para resolver esse problema que surgiram os vetores.

---

# O Problema

Imagine armazenar as notas de 100 alunos.

Sem vetores:

```python
nota1 = 8
nota2 = 7
nota3 = 9
nota4 = 10
...
nota100 = 6
```

Isso é inviável.

---

# A Solução

Utilizamos um vetor.

Python:

```python
notas = [8, 7, 9, 10, 6]
```

Agora temos:

```text
Uma variável

Vários valores
```

---

# O Que é um Vetor?

Definição:

> Um vetor é uma estrutura que armazena vários elementos do mesmo tipo de forma sequencial.

---

Visualmente:

```text
Índice:

0   1   2   3   4

↓

8 | 7 | 9 | 10 | 6
```

---

Cada posição possui:

* Índice
* Valor

---

# O Que é um Índice?

Índice é a posição do elemento.

Importante:

Na maioria das linguagens:

```text
A contagem começa em 0
```

---

Exemplo:

```python
nomes = ["Lucas", "Maria", "João"]
```

Representação:

```text
0 → Lucas

1 → Maria

2 → João
```

---

# Acessando Elementos

```python
nomes = ["Lucas", "Maria", "João"]

print(nomes[0])
```

Resultado:

```text
Lucas
```

---

Outro exemplo:

```python
print(nomes[1])
```

Resultado:

```text
Maria
```

---

# Por Que Começa em Zero?

Motivo histórico relacionado à memória dos computadores.

Internamente:

```text
Primeira posição

Deslocamento = 0
```

Por isso:

```text
Primeiro elemento = índice 0
```

---

# Vetores em Diferentes Linguagens

Python

```python
nomes = ["Lucas", "Maria", "João"]
```

---

Java

```java
String[] nomes = {
    "Lucas",
    "Maria",
    "João"
};
```

---

C

```c
char nomes[3][20];
```

---

JavaScript

```javascript
let nomes = [
    "Lucas",
    "Maria",
    "João"
];
```

---

# Alterando Valores

```python
nomes = ["Lucas", "Maria", "João"]

nomes[1] = "Ana"
```

Resultado:

```text
Lucas
Ana
João
```

---

# Obtendo o Tamanho do Vetor

Python:

```python
nomes = ["Lucas", "Maria", "João"]

print(len(nomes))
```

Resultado:

```text
3
```

---

# Percorrendo Vetores

Uma das operações mais importantes.

---

Sem loop:

```python
print(nomes[0])
print(nomes[1])
print(nomes[2])
```

---

Com loop:

```python
for nome in nomes:

    print(nome)
```

---

Resultado:

```text
Lucas
Maria
João
```

---

# Percorrendo com Índices

```python
for i in range(len(nomes)):

    print(nomes[i])
```

---

Resultado:

```text
Lucas
Maria
João
```

---

# Aplicação Real

Sistema Escolar

```python
notas = [8, 7, 10, 6, 9]
```

Calcular média:

```python
soma = 0

for nota in notas:

    soma += nota

media = soma / len(notas)

print(media)
```

---

# Inserindo Novos Valores

Python:

```python
nomes = []

nomes.append("Lucas")
nomes.append("Maria")
```

Resultado:

```text
["Lucas", "Maria"]
```

---

# Removendo Valores

```python
nomes.remove("Maria")
```

Resultado:

```text
["Lucas"]
```

---

# Busca em Vetores

Uma tarefa extremamente comum.

---

Exemplo

Encontrar número 7.

```python
numeros = [2,4,7,8,10]
```

---

Método simples:

```python
if 7 in numeros:

    print("Encontrado")
```

---

Resultado:

```text
Encontrado
```

---

# Busca Linear

Algoritmo mais básico.

---

Funcionamento:

```text
Começa no início

↓

Verifica elemento

↓

Encontrou?

↓

Sim → Para

Não → Continua
```

---

Exemplo

```python
numeros = [4,8,15,16,23,42]

procurado = 23

for numero in numeros:

    if numero == procurado:

        print("Encontrado")
```

---

# Complexidade da Busca Linear

No pior caso:

```text
Verifica todos os elementos
```

Complexidade:

```text
O(n)
```

---

# Vetores Numéricos

```python
idades = [18,20,25,30]
```

---

# Vetores de Texto

```python
nomes = [
    "Lucas",
    "Maria",
    "Pedro"
]
```

---

# Vetores Booleanos

```python
status = [
    True,
    False,
    True
]
```

---

# Vetores Mistos

Python permite:

```python
dados = [
    "Lucas",
    19,
    True
]
```

---

Mas em sistemas profissionais geralmente evitamos isso.

---

# Maior Valor do Vetor

```python
numeros = [5,7,2,10,3]

print(max(numeros))
```

Resultado:

```text
10
```

---

# Menor Valor

```python
print(min(numeros))
```

Resultado:

```text
2
```

---

# Soma dos Valores

```python
print(sum(numeros))
```

Resultado:

```text
27
```

---

# Ordenação

Python:

```python
numeros.sort()
```

---

Antes:

```text
5 7 2 10 3
```

---

Depois:

```text
2 3 5 7 10
```

---

# Vetores Bidimensionais

São conhecidos como matrizes.

Exemplo:

```python
notas = [
    [8,7],
    [10,9],
    [6,5]
]
```

---

Representação:

```text
8  7

10 9

6  5
```

---

Matrizes serão estudadas no próximo capítulo.

---

# Estudo de Caso

Cadastro de Produtos

```python
produtos = [
    "Mouse",
    "Teclado",
    "Monitor"
]
```

Listagem:

```python
for produto in produtos:

    print(produto)
```

---

# Estudo de Caso Profissional

Sistema de Estoque

```python
estoque = [
    50,
    20,
    100,
    75
]
```

Somar estoque:

```python
total = sum(estoque)

print(total)
```

---

# Erros Mais Comuns

## Erro 1

Índice inexistente.

```python
nomes = ["Lucas"]

print(nomes[5])
```

Resultado:

```text
Erro
```

---

## Erro 2

Esquecer que começa em 0.

---

Errado:

```text
Primeiro elemento = índice 1
```

---

Correto:

```text
Primeiro elemento = índice 0
```

---

## Erro 3

Modificar vetor durante loop sem cuidado.

Pode causar comportamentos inesperados.

---

# Exercícios Resolvidos

## Exercício 1

Mostrar todos os elementos.

```python
nomes = ["Ana","Lucas","Pedro"]

for nome in nomes:

    print(nome)
```

---

## Exercício 2

Somar números.

```python
numeros = [1,2,3,4,5]

print(sum(numeros))
```

---

## Exercício 3

Encontrar maior número.

```python
numeros = [5,8,2,20]

print(max(numeros))
```

---

# Exercícios

1. Criar vetor com 10 números.
2. Mostrar todos os números.
3. Mostrar apenas números pares.
4. Somar todos os elementos.
5. Calcular média.
6. Encontrar maior valor.
7. Encontrar menor valor.
8. Contar elementos.
9. Fazer busca linear.
10. Ordenar vetor.

---

# Desafio

Crie um sistema que:

1. Receba 10 notas.
2. Armazene em um vetor.
3. Calcule a média.
4. Mostre a maior nota.
5. Mostre a menor nota.
6. Mostre todas as notas em ordem crescente.

---

# Curiosidade

Vetores estão entre as estruturas mais importantes da computação.

Muitas estruturas avançadas como:

* Listas
* Pilhas
* Filas
* Tabelas
* Bancos de dados
* Sistemas operacionais

são construídas utilizando conceitos baseados em arrays e memória sequencial.

---

# Resumo do Capítulo

Você aprendeu:

* O que são vetores.
* O que são arrays.
* Índices.
* Acesso a elementos.
* Percorrer vetores.
* Inserção e remoção.
* Busca linear.
* Ordenação.
* Operações matemáticas.
* Casos reais de uso.

**Próximo capítulo:** Matrizes — tabelas bidimensionais, linhas, colunas, percorrendo matrizes, operações matemáticas e aplicações em sistemas reais.
