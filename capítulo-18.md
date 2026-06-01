# CAPÍTULO 18 — RECURSIVIDADE

## Quando uma Função Chama a Si Mesma

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o conceito de recursividade.
* Compreender quando utilizar recursão.
* Diferenciar recursão e repetição.
* Implementar funções recursivas.
* Resolver problemas clássicos utilizando recursividade.
* Entender pilha de execução (Call Stack).
* Aplicar recursão em árvores, grafos e algoritmos avançados.
* Identificar erros comuns envolvendo recursão.

---

# Introdução

Imagine duas pessoas.

A primeira pergunta:

```text
O que é recursividade?
```

A segunda responde:

```text
Para entender recursividade,
você precisa primeiro entender recursividade.
```

Parece uma brincadeira.

Mas essa frase descreve exatamente o conceito.

---

# O Que é Recursividade?

Definição:

> Recursividade é uma técnica em que uma função chama a si mesma para resolver um problema.

---

Visualmente:

```text
Função

↓

Chama ela mesma

↓

Chama ela mesma

↓

Chama ela mesma

↓

Até chegar ao fim
```

---

# Por Que Utilizar Recursão?

Alguns problemas possuem natureza recursiva.

Exemplos:

* Estruturas hierárquicas.
* Árvores.
* Sistemas de arquivos.
* Algoritmos matemáticos.
* Inteligência Artificial.
* Compiladores.

---

# Exemplo do Mundo Real

Imagine uma pasta.

Dentro dela existem:

```text
Documentos

Imagens

Outras pastas
```

---

Essas outras pastas também possuem:

```text
Documentos

Imagens

Outras pastas
```

---

E assim sucessivamente.

É uma estrutura naturalmente recursiva.

---

# Componentes da Recursão

Toda função recursiva possui:

## Caso Base

Condição que encerra a recursão.

---

## Chamada Recursiva

Momento em que a função chama ela mesma.

---

Estrutura geral:

```python
def funcao():

    if caso_base:

        return

    funcao()
```

---

# Exemplo Simples

Contagem regressiva.

```python
def contagem(numero):

    if numero == 0:

        print("Fim")

        return

    print(numero)

    contagem(numero - 1)
```

---

Executando:

```python
contagem(5)
```

---

Resultado:

```text
5
4
3
2
1
Fim
```

---

# Entendendo Passo a Passo

Primeira chamada:

```text
contagem(5)
```

---

Ela chama:

```text
contagem(4)
```

---

Depois:

```text
contagem(3)
```

---

Depois:

```text
contagem(2)
```

---

Depois:

```text
contagem(1)
```

---

Depois:

```text
contagem(0)
```

---

O caso base é atingido.

---

# O Que Acontece na Memória?

Cada chamada é colocada na pilha de execução.

---

Visualmente:

```text
contagem(5)

↓

contagem(4)

↓

contagem(3)

↓

contagem(2)

↓

contagem(1)

↓

contagem(0)
```

---

Quando termina:

```text
contagem(0)

↑

contagem(1)

↑

contagem(2)

↑

contagem(3)

↑

contagem(4)

↑

contagem(5)
```

---

# Call Stack

Também chamada de:

```text
Pilha de Chamadas
```

---

Ela guarda:

* Variáveis locais.
* Parâmetros.
* Retornos.

---

Praticamente toda linguagem utiliza uma Call Stack.

---

# Exemplo Clássico — Fatorial

Definição:

```text
5! = 5 × 4 × 3 × 2 × 1
```

Resultado:

```text
120
```

---

Implementação:

```python
def fatorial(n):

    if n == 1:

        return 1

    return n * fatorial(n - 1)
```

---

Executando:

```python
print(fatorial(5))
```

---

Resultado:

```text
120
```

---

Expansão

```text
5 * fatorial(4)

↓

5 * 4 * fatorial(3)

↓

5 * 4 * 3 * fatorial(2)

↓

5 * 4 * 3 * 2 * fatorial(1)

↓

5 * 4 * 3 * 2 * 1
```

---

# Fórmula Matemática

n! = n\cdot(n-1)!

Caso base:

```text
1! = 1
```

---

# Exemplo Clássico — Fibonacci

Sequência:

```text
0 1 1 2 3 5 8 13 21
```

---

Cada número é:

```text
Soma dos dois anteriores
```

---

Implementação:

```python
def fibonacci(n):

    if n <= 1:

        return n

    return fibonacci(n - 1) + fibonacci(n - 2)
```

---

Executando:

```python
print(fibonacci(6))
```

---

Resultado:

```text
8
```

---

# Visualização

```text
fibonacci(5)

↓

fibonacci(4)

↓

fibonacci(3)

↓

...
```

---

A árvore cresce rapidamente.

---

# Problema do Fibonacci Recursivo

É elegante.

Mas é lento.

---

Exemplo:

```text
fibonacci(40)
```

Pode realizar milhões de chamadas.

---

Por isso muitas vezes utilizamos:

```text
Memorização

ou

Programação Dinâmica
```

---

# Recursão x Loop

Loop:

```python
for i in range(10):

    print(i)
```

---

Recursão:

```python
def mostrar(i):

    if i == 10:

        return

    print(i)

    mostrar(i + 1)
```

---

Mesmo resultado.

---

# Qual é Melhor?

Depende.

---

Loops:

* Mais rápidos.
* Menor consumo de memória.

---

Recursão:

* Mais elegante.
* Mais fácil para alguns problemas.

---

# Aplicação em Árvores

Estrutura:

```text
         A

       /   \

      B     C

     / \

    D   E
```

---

Para percorrer:

```text
A

↓

B

↓

D

↓

E

↓

C
```

---

Recursão é a solução natural.

---

# Exemplo

```python
def percorrer(no):

    if no is None:

        return

    percorrer(no.esquerda)

    percorrer(no.direita)
```

---

# Aplicação em Sistemas de Arquivos

Windows:

```text
Documentos

↓

Faculdade

↓

Programação

↓

Python
```

---

Pastas dentro de pastas.

Estrutura recursiva.

---

# Aplicação em Inteligência Artificial

Algoritmos de IA utilizam recursão em:

* Árvores de decisão.
* Busca em estados.
* Jogos.
* Planejamento.

---

# Aplicação em Grafos

Problemas de navegação.

---

Exemplo:

```text
Google Maps

GPS

Redes Sociais
```

---

Utilizam algoritmos recursivos em diversas situações.

---

# Problema: Recursão Infinita

Exemplo:

```python
def erro():

    erro()
```

---

Executando:

```python
erro()
```

---

Resultado:

```text
Stack Overflow
```

---

A pilha fica cheia.

---

# Como Evitar?

Sempre possuir:

```text
Caso Base
```

---

Toda função recursiva deve responder:

```text
Quando ela para?
```

---

# Erros Mais Comuns

## Erro 1

Não criar caso base.

---

## Erro 2

Caso base impossível de alcançar.

---

Exemplo:

```python
def teste(n):

    if n == 1000:

        return

    teste(n - 1)
```

---

Se começar em:

```python
teste(10)
```

Nunca chegará a 1000.

---

## Erro 3

Excesso de chamadas.

---

Pode causar:

```text
Stack Overflow
```

---

# Exercícios Resolvidos

## Exercício 1

Contagem regressiva.

```python
def regressiva(n):

    if n == 0:

        return

    print(n)

    regressiva(n - 1)
```

---

## Exercício 2

Soma dos números.

```python
def soma(n):

    if n == 1:

        return 1

    return n + soma(n - 1)
```

---

# Exercícios

1. Contagem regressiva.
2. Contagem crescente.
3. Soma de números.
4. Potência.
5. Fatorial.
6. Fibonacci.
7. Soma de elementos de uma lista.
8. Encontrar maior valor.
9. Inverter string.
10. Contar caracteres.

---

# Desafio

Crie uma função recursiva que:

1. Receba uma lista de números.
2. Some todos os elementos.
3. Sem utilizar loops.
4. Apenas recursão.

---

# Curiosidade

A recursividade é um dos conceitos mais cobrados em entrevistas técnicas e aparece frequentemente em competições de programação, algoritmos avançados e disciplinas de Estruturas de Dados.

---

# Resumo do Capítulo

Você aprendeu:

* O que é recursividade.
* Caso base.
* Chamada recursiva.
* Pilha de execução.
* Fatorial.
* Fibonacci.
* Recursão x Loop.
* Árvores.
* Grafos.
* Aplicações reais.
