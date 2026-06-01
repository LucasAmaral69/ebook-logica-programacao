# CAPÍTULO 7 — VARIÁVEIS E CONSTANTES

## Como os Computadores Armazenam Informações

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que são variáveis.
* Compreender o conceito de memória.
* Entender o que são constantes.
* Saber quando usar cada uma.
* Criar nomes adequados para variáveis.
* Evitar erros comuns.
* Entender como os dados são armazenados internamente.
* Desenvolver uma base sólida para os próximos capítulos.

---

# Introdução

Imagine que você está organizando seu quarto.

Você possui várias caixas.

Cada caixa possui:

* Um nome.
* Um conteúdo.

Exemplo:

```text
Caixa: Roupas
Conteúdo: Camisetas
```

```text
Caixa: Livros
Conteúdo: Apostilas
```

```text
Caixa: Eletrônicos
Conteúdo: Mouse
```

As variáveis funcionam de forma muito parecida.

---

# O Que é uma Variável?

Uma variável é um espaço reservado na memória do computador para armazenar informações.

Definição simples:

> Variável é um local onde um dado pode ser armazenado e alterado durante a execução de um programa.

---

# Exemplo Simples

Imagine:

```text
Nome = Lucas
```

O computador faz algo parecido com:

```text
┌────────────┐
│ nome       │
├────────────┤
│ Lucas      │
└────────────┘
```

---

# Por Que o Nome "Variável"?

Porque o valor pode variar.

Exemplo:

Inicialmente:

```text
idade = 18
```

Depois:

```text
idade = 19
```

Depois:

```text
idade = 20
```

O valor mudou.

Por isso ela é chamada de variável.

---

# Variável na Vida Real

Pense em uma conta bancária.

Hoje:

```text
Saldo = R$ 100
```

Após um depósito:

```text
Saldo = R$ 200
```

Após uma compra:

```text
Saldo = R$ 150
```

O saldo muda constantemente.

É uma variável.

---

# Como a Memória Funciona?

Quando um programa é executado, o sistema operacional reserva uma área da memória RAM.

Dentro dessa memória, os dados são armazenados.

Exemplo:

```text
┌────────────┐
│ nome       │ → Lucas
├────────────┤
│ idade      │ → 20
├────────────┤
│ altura     │ → 1.75
└────────────┘
```

---

# Primeira Variável em Python

```python
nome = "Lucas"
```

---

Representação:

```text
nome
↓
Lucas
```

---

# Criando Diversas Variáveis

```python
nome = "Lucas"
idade = 20
altura = 1.75
```

---

Na memória:

```text
nome   → Lucas

idade  → 20

altura → 1.75
```

---

# Atribuição

O símbolo:

```python
=
```

não significa igualdade matemática.

Significa:

> Recebe um valor.

---

Exemplo:

```python
idade = 20
```

Leitura correta:

```text
idade recebe 20
```

---

# Erro Comum de Iniciantes

Muitos pensam:

```python
x = x + 1
```

é impossível.

Matematicamente seria.

Mas em programação significa:

```text
Pegue o valor atual de x

Some 1

Guarde novamente em x
```

---

Exemplo

```python
x = 5

x = x + 1
```

Resultado:

```text
x = 6
```

---

# Atualizando Variáveis

Exemplo:

```python
pontos = 0

pontos = pontos + 10

pontos = pontos + 50
```

Resultado:

```text
60 pontos
```

---

# Visualizando Passo a Passo

Estado inicial:

```text
pontos = 0
```

---

Após:

```python
pontos = pontos + 10
```

```text
pontos = 10
```

---

Após:

```python
pontos = pontos + 50
```

```text
pontos = 60
```

---

# Variáveis e Entrada de Dados

Podemos armazenar informações digitadas pelo usuário.

```python
nome = input("Digite seu nome: ")
```

---

Fluxo:

```text
Usuário digita

↓

Lucas

↓

Variável nome recebe

↓

Lucas
```

---

# Variáveis e Cálculos

Exemplo:

```python
numero1 = 10
numero2 = 20

resultado = numero1 + numero2
```

---

Memória:

```text
numero1 → 10

numero2 → 20

resultado → 30
```

---

# O Que é uma Constante?

Constante é um valor que não deve ser alterado durante o programa.

---

Definição:

> Constante é um dado cujo valor permanece fixo.

---

# Exemplo Clássico

π (Pi)

```text
3.14159265359...
```

Não muda.

---

# Exemplo em Programação

```python
PI = 3.14159
```

---

# Outro Exemplo

Dias da semana:

```python
DIAS_SEMANA = 7
```

---

Meses do ano:

```python
MESES_ANO = 12
```

---

Esses valores não costumam mudar.

---

# Convenção para Constantes

Normalmente utilizamos letras maiúsculas.

```python
PI = 3.14159

IDADE_MINIMA = 18

TAXA_JUROS = 0.15
```

---

# Convenção para Variáveis

Utilizamos letras minúsculas.

```python
nome

idade

altura

salario
```

---

# Regras para Nomes de Variáveis

---

## Correto

```python
nome

idade

salario

quantidade
```

---

## Incorreto

```python
123nome

@idade

meu salário
```

---

# Pode Começar com Número?

Não.

---

Errado:

```python
1nome = "Lucas"
```

---

Correto:

```python
nome1 = "Lucas"
```

---

# Pode Ter Espaços?

Não.

---

Errado:

```python
meu nome = "Lucas"
```

---

Correto:

```python
meu_nome = "Lucas"
```

---

# Nomes Significativos

---

Ruim:

```python
a = 10

b = 20

c = a + b
```

---

Bom:

```python
preco_produto = 10

frete = 20

valor_total = preco_produto + frete
```

---

O segundo exemplo é muito mais fácil de entender.

---

# Boas Práticas Profissionais

---

## Regra 1

Escolha nomes claros.

---

Ruim:

```python
x = 10
```

---

Bom:

```python
idade = 10
```

---

## Regra 2

Evite abreviações desnecessárias.

---

Ruim:

```python
qtd_usr
```

---

Melhor:

```python
quantidade_usuarios
```

---

## Regra 3

Seja consistente.

---

Escolha um padrão.

Mantenha o padrão.

---

# Escopo (Introdução)

Nem toda variável existe para sempre.

Exemplo:

```python
def teste():

    numero = 10
```

A variável existe apenas dentro da função.

Esse assunto será aprofundado futuramente.

---

# Tipagem e Variáveis

Uma variável pode armazenar diferentes tipos de dados.

Exemplo:

```python
nome = "Lucas"

idade = 20

altura = 1.75

ativo = True
```

---

Tipos:

```text
String

Inteiro

Float

Booleano
```

---

Esses tipos serão estudados detalhadamente no próximo capítulo.

---

# Exercício Resolvido 1

Problema:

Guardar nome e idade.

---

Solução:

```python
nome = "Maria"

idade = 25
```

---

# Exercício Resolvido 2

Problema:

Calcular salário final.

---

```python
salario = 1500

bonus = 300

salario_final = salario + bonus
```

---

Resultado:

```text
1800
```

---

# Exercício Resolvido 3

Problema:

Calcular área do círculo.

---

```python
PI = 3.14159

raio = 5

area = PI * raio * raio
```

---

Resultado:

```text
78.53975
```

---

# Erros Mais Comuns

---

## Erro 1

Nome sem significado.

---

```python
a = 10

b = 20
```

---

## Erro 2

Sobrescrever variável sem querer.

---

```python
idade = 20

idade = 5
```

---

Valor anterior foi perdido.

---

## Erro 3

Misturar significados.

---

```python
nome = "Lucas"

nome = 20
```

---

Evite fazer isso.

---

## Erro 4

Esquecer de inicializar.

---

Ruim:

```python
print(idade)
```

Sem criar idade antes.

---

# Como Linguagens Diferem

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

A lógica continua exatamente igual.

---

# Curiosidade

Grandes sistemas podem utilizar milhões de variáveis durante sua execução.

Um navegador moderno como o [Google Chrome](https://www.google.com/chrome/?utm_source=chatgpt.com) manipula milhares de estruturas de dados e variáveis simultaneamente enquanto você navega.

---

# Desafio

Crie as variáveis necessárias para representar um aluno contendo:

* Nome
* Idade
* Matrícula
* Curso
* Nota 1
* Nota 2
* Média

Depois identifique quais poderiam ser constantes dentro do sistema.

---

# Resumo do Capítulo

Você aprendeu:

* O que são variáveis.
* O que são constantes.
* Como a memória funciona.
* Como armazenar dados.
* Como atualizar valores.
* Boas práticas de nomenclatura.
* Convenções profissionais.
* Erros comuns.
* Diferenças entre variáveis e constantes.
