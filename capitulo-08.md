# CAPÍTULO 8 — TIPOS DE DADOS

## Como os Computadores Entendem e Armazenam Informações

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que são tipos de dados.
* Compreender por que eles existem.
* Conhecer os principais tipos utilizados na programação.
* Diferenciar inteiros, reais, caracteres, strings e booleanos.
* Realizar conversões entre tipos.
* Entender como os dados são armazenados na memória.
* Evitar erros comuns relacionados à tipagem.
* Compreender diferenças entre linguagens de programação.

---

# Introdução

Imagine que você possui várias caixas para guardar objetos.

Você não colocaria:

* Água dentro de uma caixa de papelão.
* Um carro dentro de uma mochila.
* Um navio dentro de uma garagem residencial.

Cada objeto exige um recipiente adequado.

Na programação ocorre exatamente a mesma coisa.

Os dados possuem tipos.

E cada tipo é armazenado de uma maneira específica.

---

# O Que é um Tipo de Dado?

Definição simples:

> Tipo de dado é uma classificação que define quais valores uma variável pode armazenar e quais operações podem ser realizadas com ela.

---

# Por Que os Tipos Existem?

Imagine o seguinte:

```text id="t4q9v2"
Nome = Lucas
```

e

```text id="u1gf0v"
Idade = 20
```

Claramente os dois valores são diferentes.

Um é texto.

Outro é número.

O computador precisa saber disso.

---

# Exemplo

```python
nome = "Lucas"

idade = 20
```

O computador identifica automaticamente:

```text
nome → texto

idade → número inteiro
```

---

# Os Principais Tipos de Dados

Quase todas as linguagens possuem:

* Inteiro (Integer)
* Real (Float/Double)
* Caractere (Char)
* String
* Booleano (Boolean)
* Nulo (Null/Nil)

---

# Inteiros (Integer)

Inteiros são números sem parte decimal.

---

Exemplos:

```text
0
1
10
500
10000
-25
-100
```

---

Variáveis inteiras:

```python
idade = 20

quantidade = 50

ano = 2026
```

---

Uso comum:

* Idade
* Quantidade
* Número de alunos
* Número de produtos
* Ano

---

# Representação na Memória

Um inteiro ocupa uma quantidade específica de bytes.

Exemplo comum:

```text
4 bytes = 32 bits
```

Isso permite armazenar aproximadamente:

```text
-2.147.483.648

até

2.147.483.647
```

---

# Exemplo em Linguagens

Python:

```python
idade = 20
```

---

Java:

```java
int idade = 20;
```

---

C:

```c
int idade = 20;
```

---

# Números Reais

Também chamados de:

* Float
* Double
* Ponto Flutuante

---

São números com casas decimais.

---

Exemplos:

```text
1.5

3.14

10.75

99.99

0.001
```

---

Python:

```python
altura = 1.75
```

---

Uso comum:

* Altura
* Peso
* Salário
* Temperatura
* Distância

---

# Problema dos Números Reais

Muitos iniciantes acreditam que números decimais são armazenados exatamente.

Nem sempre.

Exemplo:

```python
print(0.1 + 0.2)
```

Resultado:

```text
0.30000000000000004
```

---

Isso acontece devido à forma como computadores armazenam números em binário.

---

# Como Computadores Armazenam Dados

Computadores não entendem:

```text
A

B

C

1

2

3
```

Eles entendem apenas:

```text
0

1
```

Tudo é convertido para binário.

---

Exemplo:

Número 5:

```text
101
```

---

Número 10:

```text
1010
```

---

Número 20:

```text
10100
```

---

Tudo vira bits.

---

# Caractere (Char)

Representa apenas UM caractere.

---

Exemplos:

```text
A

B

C

1

@

#
```

---

Java:

```java
char letra = 'A';
```

---

C:

```c
char letra = 'A';
```

---

Importante:

```text
'A'
```

não é a mesma coisa que:

```text
"ABC"
```

---

# String

String representa uma sequência de caracteres.

---

Exemplos:

```text
"Lucas"

"Programação"

"Python"

"Olá Mundo"
```

---

Python:

```python
nome = "Lucas"
```

---

Java:

```java
String nome = "Lucas";
```

---

Uso comum:

* Nome
* Endereço
* CPF
* E-mail
* Senha
* Cidade

---

# Como Uma String é Armazenada?

Exemplo:

```text
Lucas
```

Na memória:

```text
L
u
c
a
s
```

Cada caractere possui uma posição.

---

Índices:

```text
L → 0

u → 1

c → 2

a → 3

s → 4
```

---

# Booleano (Boolean)

Um dos tipos mais importantes da programação.

---

Pode armazenar apenas:

```text
Verdadeiro

Falso
```

---

Python:

```python
ativo = True
```

---

Java:

```java
boolean ativo = true;
```

---

Uso comum:

* Usuário logado
* Sistema ativo
* Produto disponível
* Maior de idade

---

Exemplos:

```python
maior_idade = True

produto_disponivel = False
```

---

# O Tipo Nulo

Representa ausência de valor.

---

Python:

```python
nome = None
```

---

Java:

```java
String nome = null;
```

---

Exemplo:

```text
Nome ainda não informado.
```

---

# Tipagem Dinâmica e Estática

Existem dois grandes grupos de linguagens.

---

# Tipagem Dinâmica

O tipo é identificado automaticamente.

Exemplo:

Python.

```python
nome = "Lucas"

idade = 20
```

---

Não precisamos declarar tipos.

---

# Tipagem Estática

O tipo deve ser informado.

Exemplo:

Java.

```java
String nome = "Lucas";

int idade = 20;
```

---

# Comparação

Python:

```python
idade = 20
```

---

Java:

```java
int idade = 20;
```

---

C#:

```csharp
int idade = 20;
```

---

# Conversão de Tipos

Também chamada de Casting.

---

Problema:

```python
idade = "20"
```

Isto é texto.

---

Se quisermos número:

```python
idade = int("20")
```

Resultado:

```text
20
```

---

# String Para Inteiro

```python
numero = int("50")
```

---

Resultado:

```text
50
```

---

# Inteiro Para String

```python
numero = str(50)
```

---

Resultado:

```text
"50"
```

---

# Float Para Inteiro

```python
valor = int(10.9)
```

---

Resultado:

```text
10
```

---

A parte decimal é descartada.

---

# Erro Muito Comum

```python
idade = input()

resultado = idade + 10
```

Erro.

Porque:

```text
idade = texto
```

---

Correto:

```python
idade = int(input())

resultado = idade + 10
```

---

# Operações Permitidas

Inteiros:

```python
10 + 5

10 - 5

10 * 5

10 / 5
```

---

Strings:

```python
"Olá " + "Mundo"
```

Resultado:

```text
Olá Mundo
```

---

Booleanos:

```python
True and False
```

Resultado:

```text
False
```

---

# Tabela Resumo

| Tipo    | Exemplo |
| ------- | ------- |
| int     | 10      |
| float   | 10.5    |
| char    | A       |
| string  | Lucas   |
| boolean | True    |
| null    | None    |

---

# Estudo de Caso

Sistema Escolar.

Dados:

```text
Nome

Idade

Média

Aprovado
```

Tipos:

```text
Nome → String

Idade → Integer

Média → Float

Aprovado → Boolean
```

---

# Boas Práticas

---

## Use o tipo correto

Ruim:

```python
idade = "20"
```

---

Bom:

```python
idade = 20
```

---

## Não misture significados

Ruim:

```python
nome = 25
```

---

Bom:

```python
nome = "Lucas"
```

---

## Valide entradas

Antes de converter:

```python
int(valor)
```

Garanta que realmente é número.

---

# Exercícios Resolvidos

---

## Exercício 1

Crie uma variável para idade.

```python
idade = 20
```

Tipo:

```text
Integer
```

---

## Exercício 2

Crie uma variável para salário.

```python
salario = 2500.50
```

Tipo:

```text
Float
```

---

## Exercício 3

Crie uma variável para usuário ativo.

```python
ativo = True
```

Tipo:

```text
Boolean
```

---

# Exercícios

1. Crie uma variável string para seu nome.
2. Crie uma variável inteira para sua idade.
3. Crie uma variável float para sua altura.
4. Crie uma variável boolean para indicar se estuda programação.
5. Crie uma variável nula.
6. Converta string para inteiro.
7. Converta inteiro para string.
8. Converta float para inteiro.
9. Converta inteiro para float.
10. Faça cálculos utilizando diferentes tipos.


---

# Curiosidade

Toda informação armazenada em um computador — textos, vídeos, músicas, imagens e programas — é representada internamente por sequências de bits (0 e 1).

Uma foto com milhões de cores e um simples número inteiro são, no final das contas, apenas padrões diferentes de bits na memória.

---

# Resumo do Capítulo

Você aprendeu:

* O que são tipos de dados.
* Inteiros.
* Números reais.
* Caracteres.
* Strings.
* Booleanos.
* Valores nulos.
* Conversões de tipos.
* Tipagem dinâmica.
* Tipagem estática.
* Boas práticas profissionais.
