# CAPÍTULO 9 — OPERADORES

## Como os Computadores Realizam Cálculos e Tomam Decisões

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que são operadores.
* Utilizar operadores aritméticos.
* Utilizar operadores relacionais.
* Utilizar operadores lógicos.
* Utilizar operadores de atribuição.
* Compreender a precedência de operadores.
* Resolver problemas reais utilizando expressões.
* Evitar erros comuns cometidos por iniciantes.

---

# Introdução

Variáveis armazenam dados.

Mas como fazemos cálculos?

Como comparamos valores?

Como verificamos condições?

Como tomamos decisões?

A resposta está nos operadores.

---

# O Que é um Operador?

Um operador é um símbolo que realiza uma operação sobre um ou mais valores.

---

Exemplo:

```python
10 + 5
```

Neste caso:

```text
10 → Operando

+  → Operador

5  → Operando
```

Resultado:

```text
15
```

---

# Categorias de Operadores

Na maioria das linguagens existem cinco grupos principais:

1. Operadores Aritméticos
2. Operadores Relacionais
3. Operadores Lógicos
4. Operadores de Atribuição
5. Operadores de Incremento e Decremento

---

# Operadores Aritméticos

São utilizados para cálculos matemáticos.

---

## Soma

Operador:

```text
+
```

---

Exemplo:

```python
10 + 5
```

Resultado:

```text
15
```

---

## Subtração

Operador:

```text
-
```

---

Exemplo:

```python
20 - 8
```

Resultado:

```text
12
```

---

## Multiplicação

Operador:

```text
*
```

---

Exemplo:

```python
4 * 5
```

Resultado:

```text
20
```

---

## Divisão

Operador:

```text
/
```

---

Exemplo:

```python
10 / 2
```

Resultado:

```text
5
```

---

## Potência

Python:

```python
2 ** 3
```

Resultado:

```text
8
```

Representa:

```text
2³
```

---

## Resto da Divisão (Módulo)

Operador:

```text
%
```

---

Exemplo:

```python
10 % 3
```

Resultado:

```text
1
```

---

Porque:

```text
10 ÷ 3 = 3

Resto = 1
```

---

Muito utilizado para:

* Verificar números pares.
* Verificar números ímpares.
* Ciclos.
* Jogos.

---

## Divisão Inteira

Python:

```python
10 // 3
```

Resultado:

```text
3
```

A parte decimal é descartada.

---

# Exemplos Práticos

---

## Área do Retângulo

```python
base = 10

altura = 5

area = base * altura
```

Resultado:

```text
50
```

---

## Média Escolar

```python
media = (8 + 10) / 2
```

Resultado:

```text
9
```

---

# Operadores Relacionais

Utilizados para comparação.

O resultado sempre será:

```text
True

ou

False
```

---

# Igual

Operador:

```text
==
```

---

Exemplo:

```python
10 == 10
```

Resultado:

```text
True
```

---

Exemplo:

```python
10 == 20
```

Resultado:

```text
False
```

---

# Diferente

Operador:

```text
!=
```

---

Exemplo:

```python
10 != 20
```

Resultado:

```text
True
```

---

# Maior que

Operador:

```text
>
```

---

Exemplo:

```python
20 > 10
```

Resultado:

```text
True
```

---

# Menor que

Operador:

```text
<
```

---

Exemplo:

```python
5 < 10
```

Resultado:

```text
True
```

---

# Maior ou Igual

Operador:

```text
>=
```

---

Exemplo:

```python
18 >= 18
```

Resultado:

```text
True
```

---

# Menor ou Igual

Operador:

```text
<=
```

---

Exemplo:

```python
7 <= 10
```

Resultado:

```text
True
```

---

# Tabela Resumo

| Operador | Significado    |
| -------- | -------------- |
| ==       | Igual          |
| !=       | Diferente      |
| >        | Maior          |
| <        | Menor          |
| >=       | Maior ou igual |
| <=       | Menor ou igual |

---

# Aplicação Real

Sistema de aprovação.

```python
media = 8

media >= 7
```

Resultado:

```text
True
```

Aluno aprovado.

---

# Operadores Lógicos

Permitem combinar condições.

---

Imagine:

```text
Usuário correto

E

Senha correta
```

Precisamos verificar as duas condições.

---

# Operador AND

Representa:

```text
E
```

---

Tabela Verdade

| A     | B     | Resultado |
| ----- | ----- | --------- |
| True  | True  | True      |
| True  | False | False     |
| False | True  | False     |
| False | False | False     |

---

Exemplo:

```python
idade = 20

idade >= 18 and idade <= 60
```

Resultado:

```text
True
```

---

# Operador OR

Representa:

```text
OU
```

---

Tabela Verdade

| A     | B     | Resultado |
| ----- | ----- | --------- |
| True  | True  | True      |
| True  | False | True      |
| False | True  | True      |
| False | False | False     |

---

Exemplo:

```python
cargo = "admin"

cargo == "admin" or cargo == "gerente"
```

Resultado:

```text
True
```

---

# Operador NOT

Representa:

```text
NÃO
```

---

Exemplo:

```python
not True
```

Resultado:

```text
False
```

---

Outro exemplo:

```python
ativo = False

not ativo
```

Resultado:

```text
True
```

---

# Aplicação Real

Sistema de Login

```python
usuario_correto = True

senha_correta = True

usuario_correto and senha_correta
```

Resultado:

```text
True
```

Login autorizado.

---

# Operadores de Atribuição

Servem para armazenar valores.

---

## Atribuição Simples

```python
idade = 20
```

---

## Soma e Atribui

```python
pontos += 10
```

Equivale a:

```python
pontos = pontos + 10
```

---

## Subtração e Atribui

```python
saldo -= 100
```

Equivale a:

```python
saldo = saldo - 100
```

---

## Multiplicação e Atribui

```python
valor *= 2
```

Equivale a:

```python
valor = valor * 2
```

---

## Divisão e Atribui

```python
valor /= 2
```

Equivale a:

```python
valor = valor / 2
```

---

# Incremento e Decremento

Algumas linguagens possuem:

```java
i++
```

ou

```java
i--
```

---

Python não possui esses operadores.

Fazemos:

```python
i += 1
```

ou

```python
i -= 1
```

---

# Precedência dos Operadores

Nem todas as operações são executadas na ordem em que aparecem.

---

Exemplo:

```python
2 + 3 * 4
```

Resultado:

```text
14
```

---

Não é:

```text
20
```

---

Porque a multiplicação ocorre primeiro.

---

Ordem geral:

```text
1. ()

2. Potência

3. Multiplicação e divisão

4. Soma e subtração

5. Comparações

6. Operadores lógicos
```

---

# Exemplo

```python
(2 + 3) * 4
```

Resultado:

```text
20
```

---

Os parênteses têm prioridade.

---

# Erros Muito Comuns

---

## Confundir = com ==

Errado:

```python
idade = 18
```

Isto atribui valor.

Não compara.

---

Correto:

```python
idade == 18
```

Isto compara.

---

## Divisão por Zero

```python
10 / 0
```

Erro.

---

Sempre valide antes.

---

## Esquecer Parênteses

Errado:

```python
media = nota1 + nota2 / 2
```

---

Correto:

```python
media = (nota1 + nota2) / 2
```

---

# Estudo de Caso Completo

Problema:

Verificar aprovação.

Regras:

* Média ≥ 7
* Frequência ≥ 75%

---

Código:

```python
media = 8
frequencia = 80

aprovado = media >= 7 and frequencia >= 75
```

Resultado:

```text
True
```

Aluno aprovado.

---

# Exercícios Resolvidos

---

## Exercício 1

Calcular área.

```python
base = 10
altura = 5

area = base * altura
```

Resultado:

```text
50
```

---

## Exercício 2

Verificar maioridade.

```python
idade = 20

idade >= 18
```

Resultado:

```text
True
```

---

## Exercício 3

Verificar número par.

```python
numero = 8

numero % 2 == 0
```

Resultado:

```text
True
```

---

# Exercícios 

1. Some dois números.
2. Subtraia dois números.
3. Multiplique dois números.
4. Divida dois números.
5. Calcule potência.
6. Verifique se número é par.
7. Verifique se idade é maior de idade.
8. Verifique aprovação escolar.
9. Calcule desconto.
10. Calcule IMC.

---

# Desafio

Crie uma expressão que valide um usuário com as seguintes regras:

* Idade mínima de 18 anos.
* Conta ativa.
* Saldo positivo.

Utilize operadores relacionais e lógicos.

---

# Resumo do Capítulo

Você aprendeu:

* Operadores aritméticos.
* Operadores relacionais.
* Operadores lógicos.
* Operadores de atribuição.
* Precedência de operadores.
* Tabelas verdade.
* Casos de uso reais.
* Erros comuns.
* Boas práticas.
