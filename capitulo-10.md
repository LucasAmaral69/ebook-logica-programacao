# CAPÍTULO 10 — ESTRUTURAS CONDICIONAIS

## Como os Programas Tomam Decisões

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender como computadores tomam decisões.
* Utilizar estruturas IF, ELSE e ELSE IF.
* Compreender o funcionamento do SWITCH.
* Construir fluxos de decisão complexos.
* Resolver problemas reais utilizando condições.
* Evitar erros comuns em lógica condicional.
* Desenvolver sistemas que respondem de forma inteligente às entradas do usuário.

---

# Introdução

Até agora, todos os programas que criamos executavam instruções em sequência.

Exemplo:

```text
Passo 1
↓
Passo 2
↓
Passo 3
↓
Fim
```

Mas a maioria dos sistemas reais precisa tomar decisões.

Exemplos:

* Um banco precisa verificar se existe saldo suficiente.
* Um site precisa verificar se a senha está correta.
* Uma escola precisa verificar se o aluno foi aprovado.
* Um e-commerce precisa verificar se o produto está disponível.

Essas decisões são feitas através das estruturas condicionais.

---

# O Que é uma Estrutura Condicional?

Uma estrutura condicional permite que o programa execute caminhos diferentes dependendo de uma condição.

---

Exemplo da vida real

Imagine um semáforo.

```text
Se verde
    Avançar

Senão
    Parar
```

Você tomou uma decisão baseada em uma condição.

---

Na programação ocorre exatamente a mesma coisa.

---

# Estrutura IF

A estrutura IF significa:

```text
SE
```

---

Sintaxe em pseudocódigo

```text
SE condição ENTÃO

    ação

FIMSE
```

---

Exemplo

```text
SE idade >= 18 ENTÃO

    Mostrar "Maior de idade"

FIMSE
```

---

Fluxograma

```text
IDADE >= 18 ?

↓ SIM

Maior de idade
```

---

Python

```python
idade = 18

if idade >= 18:
    print("Maior de idade")
```

---

# Como o IF Funciona?

O programa avalia uma condição.

A condição deve resultar em:

```text
True
```

ou

```text
False
```

---

Exemplo

```python
idade = 20

idade >= 18
```

Resultado:

```text
True
```

Logo o bloco IF será executado.

---

Outro exemplo

```python
idade = 15

idade >= 18
```

Resultado:

```text
False
```

Nada acontece.

---

# Estrutura IF e ELSE

Nem sempre queremos executar apenas um caminho.

Muitas vezes queremos dois.

---

Exemplo:

```text
SE aprovado

    Mostrar aprovado

SENÃO

    Mostrar reprovado
```

---

Pseudocódigo

```text
SE media >= 7 ENTÃO

    Escreva "Aprovado"

SENÃO

    Escreva "Reprovado"

FIMSE
```

---

Fluxograma

```text
MÉDIA >= 7 ?

↙          ↘

SIM       NÃO

↓           ↓

APROVADO REPROVADO
```

---

Python

```python
media = 6

if media >= 7:
    print("Aprovado")
else:
    print("Reprovado")
```

---

# Exemplo Real

Sistema bancário.

---

Problema:

Permitir saque apenas se houver saldo.

---

Pseudocódigo

```text
SE saldo >= saque ENTÃO

    Realizar saque

SENÃO

    Mostrar "Saldo insuficiente"

FIMSE
```

---

Python

```python
saldo = 500
saque = 300

if saldo >= saque:
    print("Saque realizado")
else:
    print("Saldo insuficiente")
```

---

# Estrutura ELSE IF

Muitas vezes temos mais de duas possibilidades.

---

Exemplo escolar

```text
Média >= 9
Excelente

Média >= 7
Aprovado

Média < 7
Reprovado
```

---

Pseudocódigo

```text
SE media >= 9 ENTÃO

    Escreva "Excelente"

SENÃO SE media >= 7 ENTÃO

    Escreva "Aprovado"

SENÃO

    Escreva "Reprovado"

FIMSE
```

---

Python

```python
media = 8

if media >= 9:
    print("Excelente")

elif media >= 7:
    print("Aprovado")

else:
    print("Reprovado")
```

---

# Fluxo de Execução

O programa testa de cima para baixo.

---

Exemplo

```python
media = 9

if media >= 7:
    print("Aprovado")

elif media >= 9:
    print("Excelente")
```

---

Resultado:

```text
Aprovado
```

---

Por quê?

Porque a primeira condição já foi verdadeira.

A segunda nunca será avaliada.

---

# Ordem das Condições

Muito importante.

---

Errado:

```python
if media >= 7:

elif media >= 9:
```

---

Correto:

```python
if media >= 9:

elif media >= 7:
```

---

Sempre coloque as condições mais específicas primeiro.

---

# Condições Aninhadas

Uma condição dentro de outra.

---

Exemplo

```python
idade = 20

possui_carteira = True

if idade >= 18:

    if possui_carteira:

        print("Pode dirigir")
```

---

Representação

```text
IDADE >= 18 ?

↓

SIM

↓

POSSUI CNH ?

↓

SIM

↓

PODE DIRIGIR
```

---

# Exemplo Profissional

Sistema de login.

---

Regras:

* Usuário correto.
* Senha correta.

---

Código

```python
usuario = "admin"
senha = "123"

if usuario == "admin":

    if senha == "123":

        print("Acesso permitido")

    else:

        print("Senha incorreta")

else:

    print("Usuário inválido")
```

---

# Utilizando Operadores Lógicos

Podemos combinar condições.

---

Exemplo

```python
idade = 20
ativo = True

if idade >= 18 and ativo:

    print("Acesso permitido")
```

---

Explicação

As duas condições precisam ser verdadeiras.

---

# Operador OR

```python
cargo = "gerente"

if cargo == "admin" or cargo == "gerente":

    print("Acesso autorizado")
```

---

Apenas uma condição precisa ser verdadeira.

---

# Operador NOT

```python
bloqueado = False

if not bloqueado:

    print("Usuário ativo")
```

---

# O Comando SWITCH

Utilizado quando temos muitas opções fixas.

---

Exemplo

Dias da semana.

---

Pseudocódigo

```text
ESCOLHA dia

CASO 1

    Domingo

CASO 2

    Segunda

CASO 3

    Terça

FIMESCOLHA
```

---

Java

```java
switch(dia){

case 1:
    System.out.println("Domingo");
    break;

case 2:
    System.out.println("Segunda");
    break;
}
```

---

C#

```csharp
switch(dia)
{
    case 1:
        Console.WriteLine("Domingo");
        break;
}
```

---

Python

Até versões recentes não possuía switch tradicional.

Atualmente existe:

```python
match dia:

    case 1:
        print("Domingo")
```

---

# Quando Usar IF?

Use IF quando:

* Comparações forem complexas.
* Existirem intervalos.
* Existirem operadores lógicos.

---

Exemplo

```python
idade >= 18 and idade <= 60
```

---

# Quando Usar SWITCH?

Use quando:

* Existem vários valores fixos.

---

Exemplo

```text
1 → Janeiro
2 → Fevereiro
3 → Março
```

---

# Erros Comuns

---

## Erro 1

Usar = ao invés de ==

---

Errado:

```python
if idade = 18
```

---

Correto:

```python
if idade == 18
```

---

## Erro 2

Condições impossíveis

---

Exemplo

```python
if idade > 18 and idade < 10
```

Nunca será verdadeiro.

---

## Erro 3

Blocos mal organizados

---

Ruim:

```python
if idade >=18:
print("Maior")
```

---

Correto:

```python
if idade >=18:
    print("Maior")
```

---

# Estudo de Caso Completo

Sistema de Desconto

---

Regras

```text
Acima de R$1000 → 20%

Acima de R$500 → 10%

Menor que R$500 → 5%
```

---

Python

```python
valor = 800

if valor > 1000:

    desconto = 20

elif valor > 500:

    desconto = 10

else:

    desconto = 5

print(desconto)
```

---

# Exercícios Resolvidos

---

## Exercício 1

Verificar maioridade.

```python
idade = 20

if idade >= 18:
    print("Maior")
else:
    print("Menor")
```

---

## Exercício 2

Verificar número positivo.

```python
numero = 5

if numero > 0:
    print("Positivo")
else:
    print("Negativo")
```

---

## Exercício 3

Sistema de notas.

```python
media = 8

if media >= 7:
    print("Aprovado")
else:
    print("Reprovado")
```

---

# Exercícios

1. Verifique maioridade.
2. Verifique número positivo.
3. Verifique número par.
4. Verifique aprovação.
5. Verifique saldo bancário.
6. Sistema de login.
7. Sistema de desconto.
8. Sistema de frete.
9. Sistema de comissão.
10. Sistema de acesso.

---

# Desafio

Crie um sistema que classifique um aluno:

```text
Média ≥ 9 → Excelente

Média ≥ 7 → Aprovado

Média ≥ 5 → Recuperação

Menor que 5 → Reprovado
```

Utilize IF, ELSE IF e ELSE.

---

# Curiosidade

Grande parte das regras de negócios de sistemas empresariais é construída com estruturas condicionais.

Sistemas de bancos, hospitais, e-commerces e ERPs podem possuir milhares de regras condicionais diferentes para processar operações do dia a dia.

---

# Resumo do Capítulo

Você aprendeu:

* IF.
* ELSE.
* ELSE IF.
* SWITCH.
* MATCH (Python).
* Condições aninhadas.
* Operadores lógicos em decisões.
* Boas práticas.
* Erros comuns.
* Casos reais de uso.
