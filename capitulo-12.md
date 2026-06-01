# CAPÍTULO 12 — FUNÇÕES E PROCEDIMENTOS

## Como Organizar Programas de Forma Profissional

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que são funções.
* Entender o que são procedimentos.
* Compreender modularização.
* Criar funções reutilizáveis.
* Utilizar parâmetros.
* Trabalhar com valores de retorno.
* Entender escopo de variáveis.
* Organizar sistemas grandes corretamente.
* Produzir código mais limpo, profissional e fácil de manter.

---

# Introdução

Imagine que você trabalha em uma empresa de entregas.

Todos os dias você precisa:

* Calcular frete.
* Calcular desconto.
* Calcular imposto.
* Gerar nota fiscal.

Agora imagine repetir esse mesmo código centenas de vezes.

Seria um desastre.

Por isso existem as funções.

---

# O Problema da Repetição

Observe o código abaixo:

```python
nota1 = 8
nota2 = 6

media = (nota1 + nota2) / 2

print(media)

nota1 = 10
nota2 = 7

media = (nota1 + nota2) / 2

print(media)
```

Estamos repetindo a mesma lógica.

Isso gera:

* Mais erros.
* Mais trabalho.
* Menor produtividade.
* Código difícil de manter.

---

# O Que é uma Função?

Definição:

> Uma função é um bloco de código reutilizável que executa uma tarefa específica.

---

Imagine uma máquina.

Entrada:

```text
Notas
```

Processamento:

```text
Calcular média
```

Saída:

```text
Resultado
```

---

Representação:

```text
Entradas
   ↓

FUNÇÃO

   ↓

Saída
```

---

# Primeira Função

Python:

```python
def saudacao():

    print("Olá Mundo")
```

---

Para executar:

```python
saudacao()
```

Resultado:

```text
Olá Mundo
```

---

# O Que é Chamar uma Função?

Quando escrevemos:

```python
saudacao()
```

Estamos pedindo ao programa:

```text
Execute o bloco de código chamado saudacao
```

---

# Fluxo Interno

```text
Programa

↓

Encontra saudacao()

↓

Vai até a função

↓

Executa

↓

Retorna ao programa
```

---

# Funções com Parâmetros

Funções podem receber informações.

Essas informações são chamadas de parâmetros.

---

Exemplo

```python
def saudar(nome):

    print("Olá", nome)
```

---

Execução

```python
saudar("Lucas")
```

Resultado:

```text
Olá Lucas
```

---

Outro exemplo

```python
saudar("Maria")
```

Resultado:

```text
Olá Maria
```

---

Observe:

A função é a mesma.

A entrada muda.

---

# Múltiplos Parâmetros

```python
def soma(a, b):

    print(a + b)
```

---

Execução

```python
soma(10, 20)
```

Resultado:

```text
30
```

---

Outro exemplo

```python
soma(100, 50)
```

Resultado:

```text
150
```

---

# Parâmetros na Vida Real

Sistema de entrega.

---

Entradas:

```text
Peso

Distância
```

---

Processamento:

```text
Calcular frete
```

---

Saída:

```text
Valor do frete
```

---

Função:

```python
def calcular_frete(peso, distancia):
```

---

# O Que é Retorno?

Algumas funções apenas executam tarefas.

Outras produzem resultados.

---

Exemplo

```python
def soma(a, b):

    return a + b
```

---

O comando:

```python
return
```

significa:

```text
Devolver um valor
```

---

# Exemplo Completo

```python
def soma(a, b):

    return a + b

resultado = soma(10, 20)

print(resultado)
```

Resultado:

```text
30
```

---

# Diferença Entre Print e Return

Muitos iniciantes confundem.

---

Exemplo com print

```python
def soma(a, b):

    print(a + b)
```

---

Apenas mostra.

Não devolve.

---

Exemplo com return

```python
def soma(a, b):

    return a + b
```

---

Devolve o valor.

Pode ser reutilizado.

---

# Comparação

Função usando print:

```python
def soma(a,b):

    print(a+b)
```

---

Função usando return:

```python
def soma(a,b):

    return a+b
```

---

A segunda é muito mais útil.

---

# Procedimentos

Em algumas linguagens existe diferença formal entre:

```text
Função

Procedimento
```

---

Função:

Retorna valor.

---

Procedimento:

Executa tarefa.

Não retorna valor.

---

Exemplo

```python
def mostrar_menu():

    print("1 - Cadastrar")

    print("2 - Sair")
```

---

Isso é equivalente a um procedimento.

---

# Modularização

Uma das palavras mais importantes da programação.

---

Definição:

> Dividir um sistema em partes menores.

---

Sistema Escolar

---

Sem modularização:

```text
1.000 linhas em um único arquivo
```

---

Com modularização:

```text
Cadastrar aluno

Calcular média

Emitir boletim

Gerar relatório
```

Cada tarefa possui sua função.

---

# Exemplo Profissional

```python
def cadastrar_aluno():

    pass

def calcular_media():

    pass

def gerar_boletim():

    pass
```

---

Muito mais organizado.

---

# Escopo de Variáveis

Escopo define onde uma variável pode ser acessada.

---

# Variável Local

Existe apenas dentro da função.

---

Exemplo

```python
def teste():

    nome = "Lucas"

    print(nome)
```

---

Funciona:

```text
Dentro da função
```

---

Não funciona:

```python
print(nome)
```

Fora da função.

---

Erro:

```text
Variável não encontrada
```

---

# Variável Global

Existe fora das funções.

---

Exemplo

```python
nome = "Lucas"

def mostrar():

    print(nome)
```

---

A função consegue acessar.

---

# Boas Práticas

Evite abusar de variáveis globais.

Projetos grandes ficam difíceis de manter.

---

# Funções Chamando Funções

Exemplo

```python
def soma(a,b):

    return a+b

def mostrar_resultado():

    resultado = soma(10,20)

    print(resultado)
```

---

Fluxo:

```text
mostrar_resultado()

↓

soma()

↓

retorna 30

↓

mostra 30
```

---

# Valores Padrão

Python permite parâmetros padrão.

---

Exemplo

```python
def saudar(nome="Visitante"):

    print(nome)
```

---

Execução

```python
saudar()
```

Resultado:

```text
Visitante
```

---

Execução

```python
saudar("Lucas")
```

Resultado:

```text
Lucas
```

---

# Número Variável de Argumentos

Python possui:

```python
*args
```

---

Exemplo

```python
def somar(*numeros):

    return sum(numeros)
```

---

Execução

```python
somar(1,2,3,4,5)
```

Resultado:

```text
15
```

---

# Recursão (Introdução)

Uma função pode chamar a si mesma.

---

Exemplo

```python
def contagem(numero):

    if numero > 0:

        print(numero)

        contagem(numero - 1)
```

---

Resultado

```text
5
4
3
2
1
```

---

Recursão será estudada profundamente em capítulo próprio.

---

# Estudo de Caso

Sistema de Média Escolar

---

Função

```python
def calcular_media(n1, n2):

    return (n1 + n2) / 2
```

---

Uso

```python
media = calcular_media(8, 10)

print(media)
```

---

Resultado

```text
9
```

---

# Estudo de Caso Profissional

Sistema de E-commerce

---

Funções

```python
def calcular_desconto():

def calcular_frete():

def calcular_total():

def emitir_nota():
```

---

Cada responsabilidade isolada.

Esse é o padrão utilizado por empresas.

---

# Erros Comuns

---

## Erro 1

Não usar return.

---

Ruim

```python
def soma(a,b):

    print(a+b)
```

---

## Erro 2

Criar funções gigantes.

---

Ruim

```text
Função com 500 linhas
```

---

Bom

```text
Muitas funções pequenas
```

---

## Erro 3

Nomes genéricos.

---

Ruim

```python
def x():
```

---

Bom

```python
def calcular_media():
```

---

# Exercícios Resolvidos

---

## Exercício 1

Criar função de saudação.

```python
def saudar():

    print("Olá")
```

---

## Exercício 2

Função de soma.

```python
def soma(a,b):

    return a+b
```

---

## Exercício 3

Função de média.

```python
def media(a,b):

    return (a+b)/2
```

---

# Exercícios

1. Função que mostra nome.
2. Função que soma dois números.
3. Função que multiplica números.
4. Função que calcula área.
5. Função que calcula média.
6. Função para verificar maioridade.
7. Função para verificar número par.
8. Função para calcular desconto.
9. Função para calcular IMC.
10. Função para calcular frete.

---

# Desafio

Crie um sistema utilizando funções para:

* Cadastrar aluno.
* Calcular média.
* Verificar aprovação.
* Exibir resultado.

Cada tarefa deve estar em uma função diferente.

---

# Curiosidade

Sistemas modernos possuem milhares de funções.

O núcleo do [Linux Kernel](https://www.kernel.org/?utm_source=chatgpt.com) contém milhões de linhas de código distribuídas em inúmeras funções e módulos independentes para facilitar manutenção e evolução.

---

# Resumo do Capítulo

Você aprendeu:

* O que são funções.
* O que são procedimentos.
* Parâmetros.
* Retorno de valores.
* Escopo local.
* Escopo global.
* Modularização.
* Valores padrão.
* Funções chamando funções.
* Boas práticas profissionais.
