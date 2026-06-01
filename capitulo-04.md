# CAPÍTULO 4 — ALGORITMOS

## O Alicerce de Todo Programa

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender profundamente o que é um algoritmo.
* Diferenciar algoritmo de código.
* Criar algoritmos para problemas reais.
* Identificar características de um bom algoritmo.
* Desenvolver algoritmos eficientes.
* Evitar erros comuns de lógica.
* Preparar-se para fluxogramas e pseudocódigo.
* Resolver problemas antes mesmo de escrever código.

---

# Introdução

Se existe um conceito que todo programador precisa dominar, é o conceito de algoritmo.

Antes de existir:

* Python
* Java
* C
* JavaScript
* C#

Já existiam algoritmos.

Na verdade, computadores executam algoritmos.

Programadores criam algoritmos.

Linguagens apenas servem para escrever esses algoritmos.

---

# O Que é um Algoritmo?

Definição simples:

> Um algoritmo é uma sequência finita e organizada de passos para resolver um problema.

---

## Definição Técnica

Segundo a literatura de Ciência da Computação:

> Um algoritmo é um conjunto de instruções não ambíguas que transforma entradas em saídas através de um processo bem definido.

---

# Exemplo Simples

Problema:

Somar dois números.

---

Entradas:

```text
10
20
```

---

Processamento:

```text
10 + 20
```

---

Saída:

```text
30
```

---

Algoritmo:

```text
1. Receber número A
2. Receber número B
3. Somar A + B
4. Exibir resultado
```

---

# Algoritmos Estão em Todo Lugar

Muitas pessoas associam algoritmos apenas à programação.

Mas eles estão presentes em praticamente tudo.

---

## Receita de Bolo

```text
1. Separar ingredientes
2. Misturar ingredientes
3. Colocar na forma
4. Assar
5. Servir
```

---

## Escovar os Dentes

```text
1. Pegar escova
2. Colocar pasta
3. Escovar dentes
4. Enxaguar
```

---

## Fazer Login

```text
1. Informar usuário
2. Informar senha
3. Validar dados
4. Permitir acesso
```

---

Todos são algoritmos.

---

# A Origem da Palavra Algoritmo

A palavra "algoritmo" deriva do nome do matemático persa:

Muhammad ibn Musa al-Khwarizmi

Seus trabalhos matemáticos influenciaram profundamente a computação moderna.

---

# Características de um Bom Algoritmo

Um algoritmo precisa possuir algumas propriedades.

---

## 1. Ser Finito

Deve terminar.

---

Exemplo correto:

```text
1. Ler número
2. Exibir número
3. Encerrar
```

---

Exemplo incorreto:

```text
1. Repetir para sempre
2. Nunca terminar
```

---

# 2. Ser Claro

Cada passo deve ser compreensível.

---

Ruim:

```text
Faça a coisa.
```

---

Bom:

```text
Some os dois números.
```

---

# 3. Ser Ordenado

A ordem importa.

---

Errado:

```text
1. Comer bolo
2. Assar bolo
3. Fazer massa
```

---

Correto:

```text
1. Fazer massa
2. Assar bolo
3. Comer bolo
```

---

# 4. Ser Executável

As instruções precisam ser possíveis.

---

Errado:

```text
1. Voar sem equipamento
```

---

Correto:

```text
1. Entrar em um avião
```

---

# Entrada, Processamento e Saída

Todo algoritmo possui três elementos.

---

## Entrada

Dados recebidos.

Exemplo:

```text
Nome
Idade
```

---

## Processamento

Transformação dos dados.

Exemplo:

```text
Calcular idade futura
```

---

## Saída

Resultado produzido.

Exemplo:

```text
Idade daqui a 10 anos
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

# Estudo de Caso 1

Problema:

Calcular média de notas.

---

Entradas:

```text
Nota 1
Nota 2
```

---

Processamento:

```text
(nota1 + nota2) / 2
```

---

Saída:

```text
Média
```

---

Algoritmo:

```text
1. Ler nota1
2. Ler nota2
3. Somar notas
4. Dividir por 2
5. Mostrar média
```

---

# Estudo de Caso 2

Problema:

Calcular salário com bônus.

---

Entradas:

```text
Salário
Percentual bônus
```

---

Processamento:

```text
salário + bônus
```

---

Saída:

```text
Salário final
```

---

Algoritmo:

```text
1. Ler salário
2. Ler bônus
3. Calcular bônus
4. Somar salário e bônus
5. Mostrar resultado
```

---

# Como Criar Algoritmos

Programadores seguem uma sequência.

---

## Passo 1

Entender o problema.

---

## Passo 2

Identificar entradas.

---

## Passo 3

Identificar processamento.

---

## Passo 4

Identificar saídas.

---

## Passo 5

Escrever os passos.

---

# Exemplo Completo

Problema:

Calcular área de um círculo.

---

Entradas:

```text
Raio
```

---

Processamento:

Área = π × raio²

---

Saída:

```text
Área
```

---

Algoritmo:

```text
1. Ler raio
2. Calcular raio²
3. Multiplicar por π
4. Exibir área
```

---

# Algoritmos Sequenciais

São algoritmos executados passo a passo.

---

Exemplo:

```text
1. Ler nome
2. Ler idade
3. Exibir nome
4. Exibir idade
```

---

Fluxo:

```text
Passo 1
↓
Passo 2
↓
Passo 3
↓
Passo 4
```

---

# Algoritmos Condicionais

Tomam decisões.

---

Exemplo:

```text
Se idade >= 18
    Mostrar "Maior de idade"
Senão
    Mostrar "Menor de idade"
```

---

# Algoritmos Repetitivos

Executam várias vezes.

---

Exemplo:

```text
Contar de 1 até 10
```

---

Passos:

```text
1
2
3
4
...
10
```

---

Esses conceitos serão aprofundados em capítulos posteriores.

---

# Pensando Como um Programador

Problema:

Criar sistema para calcular troco.

---

Iniciante pensa:

```text
Como faço isso em Python?
```

---

Programador pensa:

```text
Quais entradas existem?
```

---

Entradas:

```text
Valor compra
Valor pago
```

---

Processamento:

```text
Valor pago - valor compra
```

---

Saída:

```text
Troco
```

---

Só depois vem o código.

---

# Erros Comuns ao Criar Algoritmos

---

## Erro 1

Começar programando.

---

Errado:

```text
Abrir VS Code
Começar a digitar
```

---

Correto:

```text
Entender problema
Planejar solução
Programar
```

---

# Erro 2

Ignorar casos especiais.

---

Problema:

Divisão.

---

Pergunta:

```text
E se o divisor for zero?
```

---

Programadores profissionais pensam nisso.

---

# Erro 3

Pular etapas.

---

Exemplo:

```text
Ler nota
Mostrar aprovação
```

---

Faltou:

```text
Calcular média
```

---

# Algoritmo vs Programa

Muitos iniciantes confundem.

---

## Algoritmo

É a solução.

---

## Programa

É a implementação da solução.

---

Exemplo:

Receita de bolo.

Receita = algoritmo.

Bolo pronto = programa executado.

---

# Exemplo em Algoritmo

```text
1. Ler dois números
2. Somar
3. Mostrar resultado
```

---

# Exemplo em Python

```python
a = int(input())
b = int(input())

print(a + b)
```

---

Mesmo algoritmo.

Implementação diferente.

---

# Boas Práticas

---

## Use linguagem simples

Ruim:

```text
Realizar procedimento matemático.
```

---

Bom:

```text
Somar números.
```

---

## Um passo por vez

Ruim:

```text
Ler número e calcular resultado e mostrar saída.
```

---

Bom:

```text
Ler número
Calcular resultado
Mostrar resultado
```

---

## Mantenha ordem lógica

Sempre.

---

# Exercícios Resolvidos

---

## Exercício 1

Problema:

Calcular dobro de um número.

---

Entradas:

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

Algoritmo:

```text
1. Ler número
2. Multiplicar por 2
3. Exibir resultado
```

---

## Exercício 2

Problema:

Converter metros para centímetros.

---

Entradas:

```text
Metros
```

---

Processamento:

```text
Metros × 100
```

---

Saída:

```text
Centímetros
```

---

Algoritmo:

```text
1. Ler metros
2. Multiplicar por 100
3. Mostrar resultado
```

---

# Exercícios Propostos

---

## Nível Básico

1. Calcular idade.
2. Calcular área de um quadrado.
3. Calcular perímetro de um retângulo.
4. Converter horas em minutos.
5. Converter Celsius para Fahrenheit.
6. Calcular desconto.
7. Calcular comissão.
8. Calcular IMC.
9. Calcular média de 4 notas.
10. Calcular consumo de combustível.

---

# Desafio de Lógica

Problema:

Você possui:

```text
Valor da compra = R$ 83,50

Valor pago = R$ 100,00
```

Crie o algoritmo completo para calcular o troco.

Não utilize código.

Apenas lógica.

---

# Curiosidade

Grandes empresas como Google, Microsoft e Amazon costumam avaliar algoritmos durante processos seletivos para cargos de desenvolvimento, muitas vezes antes mesmo de avaliar conhecimento específico em linguagens.

---

# Resumo do Capítulo

Você aprendeu:

* O que é um algoritmo.
* Como algoritmos funcionam.
* Entrada, processamento e saída.
* Características de bons algoritmos.
* Como criar algoritmos.
* Diferença entre algoritmo e programa.
* Erros comuns.
* Técnicas utilizadas por programadores profissionais.
