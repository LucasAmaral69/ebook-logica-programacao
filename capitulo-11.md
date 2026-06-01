# CAPÍTULO 11 — ESTRUTURAS DE REPETIÇÃO (LOOPS)

## Como Fazer o Computador Repetir Tarefas Automaticamente

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o conceito de repetição.
* Utilizar loops FOR.
* Utilizar loops WHILE.
* Entender o funcionamento do DO-WHILE.
* Trabalhar com contadores.
* Trabalhar com acumuladores.
* Construir algoritmos mais eficientes.
* Evitar loops infinitos.
* Resolver problemas reais utilizando repetições.

---

# Introdução

Imagine que você precise mostrar os números de 1 a 100.

Sem estruturas de repetição você teria que fazer:

```python
print(1)
print(2)
print(3)
print(4)
...
print(100)
```

Isso seria inviável.

Foi para resolver esse problema que surgiram os loops.

---

# O Que é um Loop?

Loop significa:

```text
Laço
Repetição
Iteração
```

É uma estrutura que permite executar um bloco de código várias vezes.

---

# Exemplo da Vida Real

Imagine um funcionário separando 100 caixas.

```text
Enquanto existirem caixas:

    pegar caixa

    armazenar caixa
```

Ele repete a mesma tarefa diversas vezes.

---

O computador faz exatamente isso.

---

# Tipos de Loops

As linguagens normalmente possuem:

* FOR
* WHILE
* DO-WHILE

---

# Loop FOR

O FOR é utilizado quando sabemos quantas vezes queremos repetir.

---

Exemplo

Mostrar números de 1 a 5.

---

Python

```python
for i in range(1, 6):
    print(i)
```

---

Resultado

```text
1
2
3
4
5
```

---

# Como o FOR Funciona?

Passo a passo:

```python
for i in range(1, 6):
```

---

Significa:

```text
i = 1
i = 2
i = 3
i = 4
i = 5
```

---

A cada repetição:

```text
i assume um novo valor
```

---

# Visualização

```text
i = 1
↓
Executa

i = 2
↓
Executa

i = 3
↓
Executa
```

---

# Outro Exemplo

Mostrar de 10 até 20.

```python
for i in range(10, 21):
    print(i)
```

---

# Contagem Regressiva

```python
for i in range(10, 0, -1):
    print(i)
```

Resultado:

```text
10
9
8
7
...
1
```

---

# Explicando o Terceiro Parâmetro

```python
range(início, fim, passo)
```

---

Exemplo

```python
range(0, 20, 2)
```

Resultado:

```text
0
2
4
6
8
10
12
14
16
18
```

---

# Aplicação Real

Sistema de geração de etiquetas.

```python
for etiqueta in range(1, 101):
    print("Etiqueta", etiqueta)
```

---

Gera 100 etiquetas automaticamente.

---

# Loop WHILE

O WHILE é utilizado quando não sabemos quantas repetições acontecerão.

---

Tradução:

```text
Enquanto
```

---

Exemplo

```python
contador = 1

while contador <= 5:

    print(contador)

    contador += 1
```

---

Resultado

```text
1
2
3
4
5
```

---

# Como o WHILE Funciona?

O programa verifica:

```python
contador <= 5
```

---

Se for:

```text
True
```

Continua repetindo.

---

Se for:

```text
False
```

Encerra.

---

# Fluxograma

```text
contador <= 5 ?

↓ Sim

Executa

↓

Volta

↓

contador <= 5 ?

↓

Não

↓

Fim
```

---

# Aplicação Real

Sistema de login.

```python
senha = ""

while senha != "1234":

    senha = input("Digite a senha: ")
```

---

O sistema continuará pedindo a senha até que esteja correta.

---

# Diferença Entre FOR e WHILE

FOR:

```text
Quantidade conhecida
```

---

WHILE:

```text
Quantidade desconhecida
```

---

Exemplos

FOR:

```text
Mostrar os 12 meses do ano
```

Quantidade conhecida.

---

WHILE:

```text
Esperar usuário digitar senha correta
```

Quantidade desconhecida.

---

# Loop Infinito

Um dos erros mais comuns.

---

Exemplo

```python
contador = 1

while contador <= 5:

    print(contador)
```

---

Problema:

```text
contador nunca muda
```

---

Resultado:

```text
Loop infinito
```

---

Correção

```python
contador += 1
```

---

# DO-WHILE

Existe em linguagens como:

* Java
* C
* C++
* C#

---

Funcionamento:

```text
Executa primeiro

Verifica depois
```

---

Java

```java
do {

    System.out.println("Executando");

} while(condicao);
```

---

Diferença para WHILE

WHILE:

```text
Verifica primeiro

Executa depois
```

---

DO-WHILE:

```text
Executa primeiro

Verifica depois
```

---

Exemplo

```java
int numero = 10;

do {

    System.out.println(numero);

} while(numero < 5);
```

---

Mesmo sendo falso:

```text
10 < 5
```

O código executa uma vez.

---

# Contadores

Muito utilizados em loops.

---

Exemplo

```python
contador = 0

for i in range(10):

    contador += 1
```

---

Resultado

```text
10
```

---

Contadores contam eventos.

---

# Acumuladores

Acumulam valores.

---

Exemplo

Somar números de 1 a 5.

```python
soma = 0

for i in range(1, 6):

    soma += i
```

---

Passo a passo

```text
0 + 1 = 1

1 + 2 = 3

3 + 3 = 6

6 + 4 = 10

10 + 5 = 15
```

---

Resultado

```text
15
```

---

# Exemplo Profissional

Sistema de vendas.

```python
total = 0

for venda in range(5):

    valor = float(input())

    total += valor

print(total)
```

---

O acumulador soma todas as vendas.

---

# BREAK

Permite interromper um loop.

---

Exemplo

```python
for i in range(100):

    if i == 10:

        break

    print(i)
```

---

Resultado

```text
0 até 9
```

---

O loop para imediatamente.

---

# CONTINUE

Ignora a repetição atual.

---

Exemplo

```python
for i in range(10):

    if i == 5:

        continue

    print(i)
```

---

Resultado

```text
0 1 2 3 4 6 7 8 9
```

---

O número 5 é ignorado.

---

# Loops Aninhados

Um loop dentro de outro.

---

Exemplo

```python
for linha in range(3):

    for coluna in range(3):

        print("*", end="")
```

---

Representação

```text
***
***
***
```

---

Muito usado para:

* Matrizes
* Jogos
* Tabelas
* Relatórios

---

# Exemplo: Tabuada

```python
numero = 5

for i in range(1, 11):

    print(numero * i)
```

---

Resultado

```text
5
10
15
20
...
50
```

---

# Estudo de Caso

Sistema de Caixa

---

Problema:

Somar compras.

```python
total = 0

for i in range(3):

    valor = float(input())

    total += valor

print(total)
```

---

# Exercícios Resolvidos

---

## Exercício 1

Mostrar números de 1 a 10.

```python
for i in range(1,11):

    print(i)
```

---

## Exercício 2

Somar números de 1 a 100.

```python
soma = 0

for i in range(1,101):

    soma += i

print(soma)
```

---

## Exercício 3

Contagem regressiva.

```python
for i in range(10,0,-1):

    print(i)
```

---

# Exercícios

1. Mostrar números de 1 a 20.
2. Mostrar números pares.
3. Mostrar números ímpares.
4. Fazer contagem regressiva.
5. Exibir tabuada.
6. Somar números digitados.
7. Calcular média.
8. Contar positivos.
9. Contar negativos.
10. Validar senha.

---

# Desafio

Crie um sistema que:

1. Peça 10 números ao usuário.
2. Some todos.
3. Mostre a média.
4. Mostre o maior número.
5. Mostre o menor número.

Utilize:

* FOR
* Variáveis
* Operadores
* Condicionais

---

# Erros Mais Comuns

---

## Erro 1

Loop infinito.

```python
while True:
```

Sem condição de saída.

---

## Erro 2

Esquecer atualizar contador.

```python
contador = 1

while contador <= 10:
```

---

## Erro 3

Usar FOR quando deveria usar WHILE.

Sempre analise o problema antes.

---

# Curiosidade

Muitos servidores web processam milhões de requisições utilizando loops continuamente.

Aplicações como [Instagram](https://www.instagram.com/?utm_source=chatgpt.com), [YouTube](https://www.youtube.com/?utm_source=chatgpt.com) e [Netflix](https://www.netflix.com/?utm_source=chatgpt.com) utilizam estruturas de repetição em praticamente todos os seus sistemas internos.

---

# Resumo do Capítulo

Você aprendeu:

* FOR.
* WHILE.
* DO-WHILE.
* Contadores.
* Acumuladores.
* BREAK.
* CONTINUE.
* Loops aninhados.
* Casos reais.
* Boas práticas.
* Erros comuns.
