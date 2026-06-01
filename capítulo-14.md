# CAPÍTULO 14 — MATRIZES

## Organizando Dados em Linhas e Colunas

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que é uma matriz.
* Diferenciar vetor e matriz.
* Trabalhar com linhas e colunas.
* Acessar elementos bidimensionais.
* Percorrer matrizes utilizando loops.
* Resolver problemas reais usando tabelas.
* Realizar operações matemáticas básicas com matrizes.
* Construir sistemas mais complexos.

---

# Introdução

No capítulo anterior aprendemos sobre vetores.

Um vetor funciona como uma lista:

```text
[10, 20, 30, 40]
```

Mas muitos problemas exigem organização em:

* Linhas
* Colunas

Por exemplo:

| Aluno | Nota 1 | Nota 2 |
| ----- | ------ | ------ |
| Lucas | 8      | 9      |
| Maria | 10     | 7      |
| João  | 6      | 8      |

Isso já não é um vetor.

É uma matriz.

---

# O Que é uma Matriz?

Definição:

> Uma matriz é uma estrutura de dados bidimensional composta por linhas e colunas.

---

Representação:

```text
      Colunas

      0   1   2

0    10  20  30

1    40  50  60

2    70  80  90

↑

Linhas
```

---

# Vetor x Matriz

Vetor:

```text
10 20 30 40
```

Uma dimensão.

---

Matriz:

```text
10 20

30 40
```

Duas dimensões.

---

# Primeira Matriz

Python:

```python
matriz = [

    [10, 20, 30],

    [40, 50, 60],

    [70, 80, 90]

]
```

---

Visualmente:

```text
10 20 30

40 50 60

70 80 90
```

---

# Como Funcionam os Índices

Uma matriz possui:

```text
linha

coluna
```

---

Exemplo:

```python
matriz[1][2]
```

Significa:

```text
linha 1

coluna 2
```

---

Na matriz:

```text
10 20 30

40 50 60

70 80 90
```

Resultado:

```text
60
```

---

# Acessando Elementos

```python
print(matriz[0][0])
```

Resultado:

```text
10
```

---

```python
print(matriz[2][1])
```

Resultado:

```text
80
```

---

# Entendendo Visualmente

```text
matriz[0][0] = 10

matriz[0][1] = 20

matriz[0][2] = 30

matriz[1][0] = 40

matriz[1][1] = 50

matriz[1][2] = 60
```

---

# Alterando Valores

```python
matriz[1][1] = 500
```

---

Antes:

```text
50
```

Depois:

```text
500
```

---

# Percorrendo uma Matriz

Uma matriz possui:

```text
Linhas

↓

Colunas
```

---

Precisamos de dois loops.

---

Exemplo

```python
for linha in matriz:

    for valor in linha:

        print(valor)
```

---

Resultado

```text
10
20
30
40
50
60
70
80
90
```

---

# Utilizando Índices

```python
for i in range(len(matriz)):

    for j in range(len(matriz[i])):

        print(matriz[i][j])
```

---

Representação:

```text
i → linha

j → coluna
```

---

# Aplicação Real

Boletim Escolar

```python
notas = [

    [8, 9],

    [10, 7],

    [6, 8]

]
```

---

Tabela:

```text
Aluno 1 → 8 9

Aluno 2 → 10 7

Aluno 3 → 6 8
```

---

# Calculando Média

```python
for aluno in notas:

    media = sum(aluno) / len(aluno)

    print(media)
```

---

Resultado:

```text
8.5

8.5

7.0
```

---

# Matrizes e Jogos

Jogos usam matrizes constantemente.

Exemplo:

Jogo da velha.

```text
X | O | X

O | X | O

X | O | X
```

---

Representação:

```python
tabuleiro = [

    ["X","O","X"],

    ["O","X","O"],

    ["X","O","X"]

]
```

---

# Matrizes e Planilhas

Uma planilha funciona como uma matriz gigante.

Exemplo:

```text
Produto | Quantidade

Mouse   | 10

Teclado | 20

Monitor | 5
```

---

Internamente:

```text
Linhas

Colunas
```

---

# Somando Todos os Elementos

```python
matriz = [

    [1,2],

    [3,4]

]
```

---

Código:

```python
soma = 0

for linha in matriz:

    for valor in linha:

        soma += valor
```

---

Resultado:

```text
10
```

---

# Encontrando o Maior Valor

```python
maior = matriz[0][0]

for linha in matriz:

    for valor in linha:

        if valor > maior:

            maior = valor
```

---

Resultado:

```text
Maior valor encontrado
```

---

# Contando Elementos

```python
contador = 0

for linha in matriz:

    for valor in linha:

        contador += 1
```

---

Resultado:

```text
Quantidade total de elementos
```

---

# Matriz Identidade

Muito utilizada na matemática.

Representação:

```text
1 0 0

0 1 0

0 0 1
```

---

Características:

* Diagonal principal = 1
* Restante = 0

---

# Matriz Quadrada

Mesmo número de linhas e colunas.

---

Exemplo:

```text
3 x 3

4 x 4

5 x 5
```

---

# Matriz Retangular

Linhas diferentes das colunas.

---

Exemplo:

```text
3 x 2

5 x 3

10 x 4
```

---

# Aplicação Profissional

Controle de Estoque

```python
estoque = [

    ["Mouse", 50],

    ["Teclado", 30],

    ["Monitor", 15]

]
```

---

Listagem:

```python
for item in estoque:

    print(item)
```

---

Resultado:

```text
Mouse 50

Teclado 30

Monitor 15
```

---

# Aplicação Profissional

Sistema de Assentos

Cinema:

```text
[Livre][Livre][Ocupado]

[Livre][Ocupado][Livre]

[Ocupado][Livre][Livre]
```

---

Representação:

```python
assentos = [

    [0,0,1],

    [0,1,0],

    [1,0,0]

]
```

---

# Matrizes em Inteligência Artificial

Imagens são armazenadas como matrizes.

---

Exemplo:

Imagem 3x3.

```text
255 255 255

128 128 128

0   0   0
```

---

Cada número representa um pixel.

---

# Erros Mais Comuns

---

## Erro 1

Trocar linha por coluna.

---

Errado:

```python
matriz[coluna][linha]
```

---

Correto:

```python
matriz[linha][coluna]
```

---

## Erro 2

Índice inexistente.

---

Exemplo:

```python
matriz[10][5]
```

Sem existir.

---

## Erro 3

Esquecer o segundo loop.

---

Uma matriz exige:

```text
Loop externo

↓

Loop interno
```

---

# Exercícios Resolvidos

---

## Exercício 1

Mostrar matriz.

```python
matriz = [

    [1,2],

    [3,4]

]

for linha in matriz:

    print(linha)
```

---

## Exercício 2

Somar elementos.

```python
soma = 0

for linha in matriz:

    for valor in linha:

        soma += valor
```

---

## Exercício 3

Encontrar maior valor.

```python
maior = max(max(linha) for linha in matriz)
```

---

# Exercícios 

1. Criar matriz 3x3.
2. Mostrar todos os valores.
3. Somar elementos.
4. Contar elementos.
5. Encontrar maior valor.
6. Encontrar menor valor.
7. Calcular média.
8. Mostrar diagonal principal.
9. Mostrar diagonal secundária.
10. Contar números pares.

---

# Desafio

Crie um sistema que:

1. Receba notas de 5 alunos.
2. Cada aluno possui 3 provas.
3. Armazene tudo em uma matriz.
4. Calcule a média de cada aluno.
5. Mostre aprovado ou reprovado.

---

# Curiosidade

Praticamente toda imagem digital, vídeo, planilha eletrônica e modelo de inteligência artificial utiliza matrizes internamente.

Bibliotecas famosas como [NumPy](https://numpy.org/?utm_source=chatgpt.com) e frameworks de IA como [TensorFlow](https://www.tensorflow.org/?utm_source=chatgpt.com) trabalham intensivamente com matrizes multidimensionais.

---

# Resumo do Capítulo

Você aprendeu:

* O que é uma matriz.
* Linhas e colunas.
* Índices bidimensionais.
* Percorrer matrizes.
* Operações matemáticas.
* Aplicações reais.
* Jogos.
* Sistemas empresariais.
* Uso em Inteligência Artificial.
