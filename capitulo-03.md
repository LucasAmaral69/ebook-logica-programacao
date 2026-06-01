# CAPÍTULO 3 — RESOLUÇÃO DE PROBLEMAS

## A Habilidade Mais Importante de Um Programador

---

# Objetivos do Capítulo

Ao final deste capítulo você será capaz de:

* Entender o que realmente significa resolver problemas.
* Aprender uma metodologia profissional para solução de problemas.
* Identificar entradas, processamento e saídas.
* Evitar erros comuns de iniciantes.
* Transformar problemas do mundo real em algoritmos.
* Melhorar significativamente seu raciocínio lógico.
* Desenvolver uma mentalidade analítica utilizada por programadores profissionais.

---

# Introdução

Existe uma frase muito conhecida entre desenvolvedores:

> "Programação não é sobre código. É sobre resolver problemas."

Muitas pessoas acreditam que programadores passam o dia escrevendo código.

Na realidade, grande parte do trabalho consiste em:

* Entender problemas.
* Analisar cenários.
* Tomar decisões.
* Planejar soluções.
* Corrigir falhas.

O código é apenas a implementação da solução.

---

# O Que é um Problema?

Um problema é qualquer situação onde existe uma diferença entre o estado atual e o estado desejado.

Exemplo:

Estado atual:

```text
Você possui 3 notas.
```

Estado desejado:

```text
Você deseja calcular a média.
```

Problema:

```text
Como calcular a média?
```

---

## Outro Exemplo

Estado atual:

```text
Uma loja possui centenas de produtos.
```

Estado desejado:

```text
Encontrar rapidamente um produto.
```

Problema:

```text
Como localizar esse produto?
```

---

# O Ciclo da Resolução de Problemas

Todo problema pode ser resolvido seguindo um processo.

Programadores experientes utilizam uma sequência semelhante à seguinte:

```text
Entender o problema
↓
Analisar informações
↓
Planejar solução
↓
Criar algoritmo
↓
Implementar código
↓
Testar
↓
Corrigir erros
↓
Finalizar
```

---

# O Erro Mais Comum dos Iniciantes

Imagine a situação:

Professor:

```text
Crie um sistema para calcular média escolar.
```

Iniciante:

```text
Abre o VS Code imediatamente.
```

Isso normalmente gera problemas.

Porque antes de programar é necessário compreender o problema.

---

# Método E.P.S

Durante todo o ebook utilizaremos um método chamado:

```text
E = Entrada
P = Processamento
S = Saída
```

Este é um dos conceitos mais importantes da lógica.

---

# Entrada

São os dados recebidos pelo programa.

Exemplo:

Calcular média.

Entradas:

```text
Nota 1
Nota 2
```

---

# Processamento

São os cálculos ou operações realizadas.

Processamento:

```text
Somar as notas
Dividir por 2
```

---

# Saída

É o resultado produzido.

Saída:

```text
Média final
```

---

# Exemplo Completo

Problema:

Calcular idade.

---

Entrada:

```text
Ano de nascimento
Ano atual
```

---

Processamento:

```text
Ano atual - Ano nascimento
```

---

Saída:

```text
Idade
```

---

Representação:

```text
ENTRADA
↓
PROCESSAMENTO
↓
SAÍDA
```

---

# Exemplo Prático 1

Problema:

Calcular área de um retângulo.

---

Entrada:

```text
Base
Altura
```

---

Processamento:

```text
Área = Base × Altura
```

---

Saída:

```text
Área calculada
```

---

# Exemplo em Pseudocódigo

```text
INÍCIO

Leia base
Leia altura

area ← base * altura

Escreva area

FIM
```

---

# Exemplo em Python

```python
base = float(input("Base: "))
altura = float(input("Altura: "))

area = base * altura

print(area)
```

---

# Técnica da Caixa Preta

Uma técnica muito utilizada é imaginar o programa como uma caixa.

```text
ENTRADA
↓
┌───────────┐
│ PROGRAMA  │
└───────────┘
↓
SAÍDA
```

---

Exemplo:

```text
10
20
↓
┌───────────┐
│ SOMA      │
└───────────┘
↓
30
```

---

# Aprendendo a Fazer Perguntas

Ao receber um problema, faça perguntas.

Exemplo:

Criar sistema de alunos.

Perguntas:

* Quantos alunos?
* Quais dados serão armazenados?
* Haverá notas?
* Haverá aprovação?
* Haverá relatório?

Quanto mais perguntas, melhor a solução.

---

# O Processo de Análise

Profissionais analisam problemas antes de programar.

---

## Exemplo

Problema:

Sistema de biblioteca.

---

Primeira análise:

Quais informações serão armazenadas?

Possíveis respostas:

```text
Título
Autor
Ano
ISBN
Quantidade
```

---

Segunda análise:

Quais operações serão necessárias?

```text
Cadastrar
Editar
Excluir
Pesquisar
Emprestar
Devolver
```

---

Agora o problema está muito mais claro.

---

# Dividindo Problemas Grandes

Um dos maiores segredos da programação é:

> Problemas grandes devem ser quebrados em pequenos problemas.

---

Problema:

Criar um aplicativo semelhante ao Uber.

Parece impossível.

---

Divisão:

```text
Login
Cadastro
Mapa
Motoristas
Pagamento
Corridas
Avaliações
```

Agora parece muito mais simples.

---

# A Regra dos Programadores Experientes

Se um problema parece difícil demais:

Divida novamente.

---

Exemplo

Módulo de Login.

Pode ser dividido em:

```text
Receber usuário
Receber senha
Validar usuário
Validar senha
Permitir acesso
```

---

# Pensando em Casos Especiais

Programadores iniciantes resolvem apenas o cenário ideal.

Programadores experientes pensam nos erros.

---

Exemplo

Problema:

Dividir dois números.

---

Iniciante:

```python
resultado = a / b
```

---

Profissional:

Pergunta:

```text
E se b for zero?
```

---

Esse tipo de pensamento evita falhas.

---

# Exemplo de Análise Completa

Problema:

Sistema de saque bancário.

---

Entradas:

```text
Saldo
Valor do saque
```

---

Processamento:

```text
Verificar saldo
Subtrair valor
```

---

Saídas:

```text
Saque realizado
ou
Saldo insuficiente
```

---

Casos especiais:

```text
Valor negativo
Saldo insuficiente
Valor zero
```

---

# O Conceito de Restrição

Todo problema possui limitações.

---

Exemplo

Sistema de notas.

Regra:

```text
Nota mínima = 0
Nota máxima = 10
```

---

Essas são restrições.

---

# Como Resolver Qualquer Problema

Passo 1

Entender problema.

---

Passo 2

Identificar entradas.

---

Passo 3

Identificar processamento.

---

Passo 4

Identificar saída.

---

Passo 5

Identificar restrições.

---

Passo 6

Criar algoritmo.

---

Passo 7

Implementar código.

---

Passo 8

Testar.

---

# Estudo de Caso Completo

Problema:

Calcular desconto de um produto.

---

Entradas:

```text
Preço original
Percentual de desconto
```

---

Processamento:

```text
Desconto = preço × percentual

Preço final = preço - desconto
```

---

Saída:

```text
Preço final
```

---

Pseudocódigo:

```text
INÍCIO

Leia preco

Leia desconto

valorDesconto ← preco * desconto / 100

precoFinal ← preco - valorDesconto

Escreva precoFinal

FIM
```

---

Python:

```python
preco = float(input("Preço: "))
desconto = float(input("Desconto (%): "))

valor_desconto = preco * desconto / 100

preco_final = preco - valor_desconto

print("Preço final:", preco_final)
```

---

# Técnicas Utilizadas por Programadores Profissionais

## Técnica 1 — Papel e Caneta

Antes do código:

Escreva.

Desenhe.

Planeje.

---

## Técnica 2 — Fluxos

Desenhe etapas.

Exemplo:

```text
Login
↓
Senha correta?
↓
Sim → Entrar
Não → Erro
```

---

## Técnica 3 — Exemplos Reais

Teste mentalmente.

---

Exemplo

```text
Nota1 = 8
Nota2 = 10

Média = 9
```

Verifique se sua lógica funciona.

---

# Debug Mental

Antes de executar código, simule.

---

Exemplo:

```python
numero = 5

numero = numero + 3

numero = numero * 2
```

---

Simulação:

```text
5
↓
8
↓
16
```

Resultado:

```text
16
```

---

Essa habilidade é extremamente importante.

---

# Exercícios Resolvidos

## Exercício 1

Problema:

Calcular dobro de um número.

---

Entrada:

```text
Número
```

---

Processamento:

```text
Número × 2
```

---

Saída:

```text
Dobro
```

---

## Exercício 2

Problema:

Converter horas em minutos.

---

Entrada:

```text
Horas
```

---

Processamento:

```text
Horas × 60
```

---

Saída:

```text
Minutos
```

---

# Exercícios Propostos

## Nível Básico

1. Calcular perímetro de um quadrado.
2. Calcular idade.
3. Converter metros para centímetros.
4. Calcular área de um círculo.
5. Calcular salário mensal.

---

## Nível Intermediário

6. Calcular média de 4 notas.
7. Verificar aprovação.
8. Calcular IMC.
9. Calcular desconto.
10. Calcular comissão de vendas.

---

## Nível Avançado

11. Sistema de caixa eletrônico.
12. Sistema de biblioteca.
13. Sistema de estacionamento.
14. Sistema de hotel.
15. Sistema de estoque.

---

# Erros Mais Comuns

## Erro 1

Não entender o problema.

---

## Erro 2

Ignorar restrições.

---

## Erro 3

Programar antes de planejar.

---

## Erro 4

Não testar.

---

## Erro 5

Não dividir problemas grandes.

---

# Curiosidade

Em grandes empresas de tecnologia, boa parte do tempo de desenvolvimento não é gasta escrevendo código.

É gasta:

* Entendendo requisitos.
* Planejando soluções.
* Analisando cenários.
* Identificando riscos.

Por isso a habilidade de resolver problemas costuma ser mais valorizada do que decorar sintaxe.

---

# Resumo do Capítulo

Neste capítulo você aprendeu:

* O que é um problema.
* Como programadores resolvem problemas.
* O modelo Entrada → Processamento → Saída.
* Como analisar requisitos.
* Como dividir problemas grandes.
* Como identificar restrições.
* Como pensar em casos especiais.
* Como planejar antes de programar.
* Como desenvolver raciocínio lógico profissional.
