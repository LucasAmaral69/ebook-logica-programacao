# CAPÍTULO 6 — PSEUDOCÓDIGO

## A Ponte Entre a Lógica e a Programação

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que é pseudocódigo.
* Compreender por que ele é utilizado.
* Escrever algoritmos de forma profissional.
* Converter problemas em pseudocódigo.
* Transformar pseudocódigo em código real.
* Desenvolver raciocínio lógico mais rapidamente.
* Preparar-se para qualquer linguagem de programação.
* Criar soluções antes de programar.

---

# Introdução

Nos capítulos anteriores aprendemos:

* Pensamento Computacional
* Resolução de Problemas
* Algoritmos
* Fluxogramas

Agora chegamos a uma das ferramentas mais importantes da lógica de programação:

> O pseudocódigo.

O pseudocódigo é considerado a ponte entre a lógica humana e a linguagem de programação.

---

# O Que é Pseudocódigo?

Pseudocódigo é uma forma de descrever algoritmos utilizando uma linguagem próxima do português, porém organizada de maneira semelhante à programação.

---

## Definição Simples

Enquanto um algoritmo pode ser escrito de maneira totalmente textual:

```text id="6m3jpo"
1. Ler nome

2. Mostrar nome

3. Encerrar
```

O pseudocódigo possui uma estrutura mais organizada:

```text id="7vl8km"
INÍCIO

Leia nome

Escreva nome

FIM
```

---

# Por Que o Pseudocódigo Existe?

Imagine aprender programação diretamente em Java.

Você teria que aprender:

* Sintaxe
* Regras
* Palavras reservadas
* Tipos
* Estruturas

Tudo ao mesmo tempo.

Isso dificulta o aprendizado.

---

O pseudocódigo resolve esse problema.

Ele permite focar apenas na lógica.

---

# Vantagens do Pseudocódigo

---

## 1. Independente da Linguagem

Um mesmo pseudocódigo pode ser convertido para:

* Python
* Java
* JavaScript
* C
* C++
* C#

---

## 2. Fácil de Ler

Mesmo quem nunca programou consegue entender.

---

## 3. Facilita o Planejamento

Muitos desenvolvedores escrevem a lógica antes do código.

---

## 4. Reduz Erros

Erros lógicos são identificados mais cedo.

---

# Estrutura Básica

A estrutura mais comum é:

```text id="97qj8d"
INÍCIO

comandos

FIM
```

---

# Primeiro Exemplo

Problema:

Exibir mensagem.

---

Pseudocódigo:

```text id="ax1a2m"
INÍCIO

Escreva "Olá Mundo"

FIM
```

---

# Comparação com Python

```python id="v0gxvr"
print("Olá Mundo")
```

---

Observe que a lógica é a mesma.

---

# Entrada de Dados

Uma das operações mais comuns é receber informações.

---

Exemplo:

```text id="t1fjlwm"
INÍCIO

Leia nome

FIM
```

---

Significado:

O programa está esperando um valor.

---

Python:

```python id="lp1t2r"
nome = input()
```

---

# Saída de Dados

Mostrar informações ao usuário.

---

Pseudocódigo:

```text id="u7zqsv"
INÍCIO

Escreva "Bem-vindo"

FIM
```

---

Python:

```python id="fj8mns"
print("Bem-vindo")
```

---

# Variáveis no Pseudocódigo

Variáveis armazenam dados.

---

Exemplo:

```text id="rj8twd"
idade ← 20
```

---

O símbolo:

```text id="3o8o6q"
←
```

significa:

"Atribuir valor."

---

Leitura correta:

```text id="aq92d7"
idade recebe 20
```

---

# Exemplo Completo

Problema:

Ler nome e mostrar nome.

---

Pseudocódigo:

```text id="z7h4ju"
INÍCIO

Leia nome

Escreva nome

FIM
```

---

# Operações Matemáticas

O pseudocódigo utiliza operadores semelhantes às linguagens.

---

Soma

```text id="byr9mw"
+
```

Subtração

```text id="o6nznn"
-
```

Multiplicação

```text id="s0ot7r"
*
```

Divisão

```text id="it0ivd"
/
```

---

# Exemplo

Problema:

Somar dois números.

---

Pseudocódigo:

```text id="8qyv7h"
INÍCIO

Leia numero1

Leia numero2

soma ← numero1 + numero2

Escreva soma

FIM
```

---

Python:

```python id="ybj7hn"
numero1 = int(input())
numero2 = int(input())

soma = numero1 + numero2

print(soma)
```

---

# Estruturas Condicionais

Tomada de decisão.

---

Problema:

Verificar maioridade.

---

Pseudocódigo:

```text id="p5l9uw"
INÍCIO

Leia idade

SE idade >= 18 ENTÃO

    Escreva "Maior de idade"

SENÃO

    Escreva "Menor de idade"

FIMSE

FIM
```

---

Python:

```python id="wl4jhg"
idade = int(input())

if idade >= 18:
    print("Maior de idade")
else:
    print("Menor de idade")
```

---

# Estrutura Condicional Completa

Problema:

Avaliar nota.

---

Pseudocódigo:

```text id="l48ryr"
INÍCIO

Leia nota

SE nota >= 90 ENTÃO

    Escreva "Excelente"

SENÃO SE nota >= 70 ENTÃO

    Escreva "Bom"

SENÃO

    Escreva "Reprovado"

FIMSE

FIM
```

---

# Estruturas de Repetição

Permitem repetir comandos.

---

# Enquanto

Executa enquanto uma condição for verdadeira.

---

Exemplo

Contar até 5.

---

Pseudocódigo:

```text id="f4ybew"
INÍCIO

contador ← 1

ENQUANTO contador <= 5 FAÇA

    Escreva contador

    contador ← contador + 1

FIMENQUANTO

FIM
```

---

Python:

```python id="g3xsn5"
contador = 1

while contador <= 5:

    print(contador)

    contador += 1
```

---

# Para

Utilizado quando sabemos quantas repetições serão feitas.

---

Pseudocódigo:

```text id="t08i9j"
INÍCIO

PARA i ← 1 ATÉ 10 FAÇA

    Escreva i

FIMPARA

FIM
```

---

Python:

```python id="kqqfdy"
for i in range(1,11):

    print(i)
```

---

# Exercício Resolvido

Problema:

Calcular média.

---

Pseudocódigo:

```text id="gq3wzn"
INÍCIO

Leia nota1

Leia nota2

media ← (nota1 + nota2) / 2

Escreva media

FIM
```

---

Python:

```python id="n3h7s7"
nota1 = float(input())
nota2 = float(input())

media = (nota1 + nota2) / 2

print(media)
```

---

# Estudo de Caso

Sistema de Caixa Eletrônico

---

Entradas:

```text id="n1p0gn"
Saldo

Valor saque
```

---

Processamento:

Verificar saldo.

---

Pseudocódigo:

```text id="rjjc8m"
INÍCIO

Leia saldo

Leia saque

SE saque <= saldo ENTÃO

    saldo ← saldo - saque

    Escreva "Saque realizado"

SENÃO

    Escreva "Saldo insuficiente"

FIMSE

FIM
```

---

# Boas Práticas

---

## Use Nomes Claros

Ruim:

```text id="zv58tp"
a

b

x
```

---

Bom:

```text id="p65hcb"
idade

salario

quantidade
```

---

## Indente Blocos

Ruim:

```text id="4z25eb"
SE idade >=18

Escreva "Maior"
```

---

Bom:

```text id="vfug1k"
SE idade >=18

    Escreva "Maior"

FIMSE
```

---

## Um Comando Por Linha

Evita confusão.

---

# Erros Comuns

---

## Erro 1

Misturar linguagens.

---

Ruim:

```text id="ksv40r"
SE idade > 18 {

print("Maior")
}
```

---

Isso não é pseudocódigo.

---

# Erro 2

Não fechar estruturas.

---

Errado:

```text id="g0y9cf"
SE idade >=18

Escreva "Maior"
```

---

Correto:

```text id="tpp8kx"
SE idade >=18

Escreva "Maior"

FIMSE
```

---

# Erro 3

Criar lógica confusa.

Sempre simplifique.

---

# Como Universidades Utilizam Pseudocódigo

Muitos cursos utilizam ferramentas como:

* Portugol
* VisualG
* Portugol Studio

Porque permitem focar primeiro na lógica.

---

## Ferramentas Recomendadas

### VisualG

Ferramenta clássica para aprender lógica.

[VisualG](https://visualg3.com.br/?utm_source=chatgpt.com)

---

### Portugol Studio

Muito utilizada em cursos técnicos e faculdades.

[Portugol Studio](https://portugolstudio.cubos.io/?utm_source=chatgpt.com)

---

# Exercícios


1. Ler nome e mostrar nome.
2. Somar dois números.
3. Calcular idade.
4. Converter metros para centímetros.
5. Calcular área de um quadrado.
6. Calcular média de quatro notas.
7. Verificar aprovação.
8. Verificar número par ou ímpar.
9. Calcular desconto.
10. Calcular IMC.


---

# Desafio

Crie o pseudocódigo completo para um sistema de cadastro de alunos contendo:

* Nome
* Idade
* Nota 1
* Nota 2
* Média
* Situação (Aprovado/Reprovado)

---

# Resumo do Capítulo

Você aprendeu:

* O que é pseudocódigo.
* Como escrever pseudocódigo.
* Entrada e saída de dados.
* Variáveis.
* Operações matemáticas.
* Condicionais.
* Repetições.
* Boas práticas.
* Conversão entre pseudocódigo e Python.

