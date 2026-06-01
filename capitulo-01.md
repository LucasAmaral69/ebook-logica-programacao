# CAPÍTULO 1 — INTRODUÇÃO À LÓGICA DE PROGRAMAÇÃO

## Do Pensamento Humano ao Computador

---

# Objetivos deste Capítulo

Ao finalizar este capítulo, você será capaz de:

* Entender o que é lógica.
* Compreender o que é lógica de programação.
* Diferenciar lógica de linguagem de programação.
* Entender como um computador "pensa".
* Conhecer os principais erros cometidos por iniciantes.
* Desenvolver uma mentalidade voltada para resolução de problemas.
* Compreender o conceito de algoritmo.
* Iniciar seu desenvolvimento como programador.

---

# O que é Lógica?

A lógica existe muito antes dos computadores.

Ela está presente em praticamente tudo que fazemos.

Quando você decide qual roupa usar, qual caminho seguir para o trabalho ou faculdade, ou como resolver um problema do dia a dia, você está utilizando lógica.

De forma simples:

> Lógica é a capacidade de organizar pensamentos e ações para alcançar um objetivo.

---

## Exemplo 1: Fazendo um Sanduíche

Imagine que você quer fazer um sanduíche.

Você não simplesmente pega tudo aleatoriamente.

Existe uma sequência:

1. Pegar o pão.
2. Abrir o pão.
3. Colocar o recheio.
4. Fechar o pão.
5. Comer.

Isso é um processo lógico.

Se invertermos os passos:

1. Comer.
2. Colocar recheio.
3. Abrir pão.

O resultado não funciona.

A ordem importa.

---

## Exemplo 2: Indo para o Trabalho

Você acorda.

Pensa:

* Tenho combustível?
* Está chovendo?
* Vou de carro ou ônibus?

Você toma decisões baseadas em condições.

Isso é exatamente o que um programa faz.

---

# O que é Lógica de Programação?

Lógica de programação é a aplicação da lógica para resolver problemas usando computadores.

Ela define como criar uma sequência de instruções que um computador possa executar.

Em outras palavras:

> Lógica de programação é a arte de transformar problemas em passos que uma máquina consegue entender.

---

# O Maior Erro dos Iniciantes

Muitas pessoas começam estudando:

* Python
* Java
* JavaScript
* C#
* C++

Mas ignoram a lógica.

O resultado normalmente é:

* Decoram código.
* Copiam exemplos.
* Não conseguem criar projetos próprios.
* Travam em entrevistas.
* Desistem da programação.

---

## Analogia da Construção

Imagine uma casa.

Você pode comprar:

* Tijolos
* Cimento
* Telhas

Mas sem projeto a casa não fica de pé.

Na programação:

* Linguagem = ferramentas
* Lógica = projeto

Sem lógica, a linguagem não resolve nada.

---

# Linguagem de Programação NÃO é Programação

Essa frase pode parecer estranha.

Mas é extremamente importante.

Programação não é saber Python.

Programação não é saber Java.

Programação não é saber JavaScript.

Programação é resolver problemas.

A linguagem é apenas o meio utilizado.

---

## Exemplo

Imagine o seguinte problema:

"Calcular a média de duas notas."

A lógica será:

1. Receber nota 1.
2. Receber nota 2.
3. Somar as notas.
4. Dividir por 2.
5. Mostrar resultado.

Essa lógica é a mesma em qualquer linguagem.

---

### Python

```python
nota1 = 8
nota2 = 10

media = (nota1 + nota2) / 2

print(media)
```

---

### Java

```java
double nota1 = 8;
double nota2 = 10;

double media = (nota1 + nota2) / 2;

System.out.println(media);
```

---

### C

```c
float nota1 = 8;
float nota2 = 10;

float media = (nota1 + nota2) / 2;

printf("%f", media);
```

---

A lógica é idêntica.

Só muda a sintaxe.

---

# Como o Computador Pensa?

Resposta curta:

Ele não pensa.

---

Muitas pessoas imaginam que o computador entende contexto.

Ele não entende.

Ele apenas executa instruções.

Por exemplo:

```python
print("Olá")
```

O computador não sabe o que significa "Olá".

Ele apenas segue instruções.

---

# O Computador é Extremamente Burro

Isso não é uma crítica.

É uma característica.

O computador:

* Não deduz.
* Não interpreta.
* Não adivinha.
* Não completa raciocínios.

Ele executa exatamente o que você pediu.

---

## Exemplo

Imagine que você programa:

```python
idade = 17

if idade > 18:
    print("Pode dirigir")
```

Resultado?

Nada acontece.

Por quê?

Porque 17 não é maior que 18.

O computador não pensa:

"Ah, está quase."

Ele apenas verifica a condição.

---

# A Precisão é Fundamental

Um pequeno erro pode causar grandes problemas.

Exemplo:

```python
saldo = 100
saque = 1000

saldo = saldo - saque
```

Resultado:

```python
-900
```

O computador não questiona:

"Tem certeza que pode sacar?"

Ele apenas executa.

---

# Pensamento Computacional

Antes de programar, precisamos aprender a pensar como solucionadores de problemas.

Isso é chamado de Pensamento Computacional.

Ele é composto por quatro pilares:

---

## 1. Decomposição

Quebrar problemas grandes em problemas menores.

---

### Problema

Criar um aplicativo de delivery.

Muito complexo.

---

Dividindo:

* Cadastro de usuários
* Cadastro de restaurantes
* Carrinho
* Pagamento
* Entrega

Agora ficou mais simples.

---

## 2. Reconhecimento de Padrões

Identificar repetições.

Exemplo:

Instagram

Facebook

TikTok

Todos possuem:

* Login
* Senha
* Perfil

Os padrões se repetem.

---

## 3. Abstração

Ignorar detalhes irrelevantes.

Imagine um sistema escolar.

Importa:

* Nome
* Nota
* Matrícula

Não importa:

* Cor do tênis do aluno

---

## 4. Algoritmos

Criar sequência de passos.

Esse é o pilar mais importante para iniciantes.

---

# O que é um Problema?

Programar é resolver problemas.

Mas o que é um problema?

Um problema é a diferença entre:

Estado atual

e

Estado desejado

---

Exemplo:

Estado atual:

Você tem R$ 0.

Estado desejado:

Você quer calcular o salário.

Problema:

Criar um sistema que faça esse cálculo.

---

# Como Resolver Problemas?

Método profissional:

1. Entender problema.
2. Identificar entradas.
3. Identificar processamento.
4. Identificar saída.
5. Criar algoritmo.
6. Implementar.

---

# Exemplo Completo

Problema:

Calcular média escolar.

---

## Entradas

* Nota 1
* Nota 2

---

## Processamento

Somar notas.

Dividir por 2.

---

## Saída

Média final.

---

Representação:

```text
ENTRADA

nota1
nota2

PROCESSAMENTO

media = (nota1 + nota2)/2

SAÍDA

media
```

---

# O Que é um Algoritmo?

Definição formal:

> Um algoritmo é uma sequência finita e ordenada de passos para resolver um problema.

---

# Características de um Algoritmo

Um algoritmo precisa ser:

### Finito

Deve terminar.

---

### Claro

Não pode gerar dúvidas.

---

### Ordenado

Os passos devem seguir sequência lógica.

---

### Executável

Deve poder ser realizado.

---

# Exemplo de Algoritmo

Problema:

Escovar os dentes.

---

Algoritmo:

1. Pegar escova.
2. Colocar pasta.
3. Escovar dentes.
4. Enxaguar boca.
5. Guardar escova.

---

# Exemplo de Algoritmo Ruim

1. Escovar.
2. Comprar pasta.
3. Enxaguar.

Não faz sentido.

---

# Algoritmos Estão em Todo Lugar

Quando você:

* Faz café
* Liga o computador
* Usa elevador
* Faz login

Existe um algoritmo.

---

# Programação é Tradução

O programador não cria mágica.

Ele traduz problemas.

---

Problema:

Somar números.

---

Lógica:

```text
Receber número A
Receber número B
Somar
Mostrar resultado
```

---

Código:

```python
a = int(input())
b = int(input())

print(a + b)
```

---

# Os 5 Níveis de Evolução do Programador

## Nível 1

Copia código.

Não entende.

---

## Nível 2

Entende exemplos simples.

---

## Nível 3

Consegue modificar exemplos.

---

## Nível 4

Consegue criar soluções próprias.

---

## Nível 5

Resolve problemas inéditos.

---

O objetivo deste ebook é levar você ao nível 5.

---

# Erros Mais Comuns dos Iniciantes

## Erro 1

Aprender sintaxe sem lógica.

---

## Erro 2

Assistir aulas sem praticar.

---

## Erro 3

Copiar projetos.

---

## Erro 4

Ter medo de errar.

---

## Erro 5

Pular fundamentos.

---

# Exercícios de Raciocínio

## Exercício 1

Escreva o algoritmo para:

Tomar banho.

---

## Exercício 2

Escreva o algoritmo para:

Fazer um miojo.

---

## Exercício 3

Escreva o algoritmo para:

Entrar em uma rede social.

---

## Exercício 4

Liste:

Entradas

Processamento

Saída

para o problema:

"Calcular o troco de uma compra."

---

## Exercício 5

Liste:

Entradas

Processamento

Saída

para:

"Cálculo da idade."

---

# Exercícios Desafio

## Desafio 1

Como você explicaria para alguém que nunca viu um computador o processo de enviar uma mensagem no WhatsApp?

Crie um algoritmo detalhado.

---

## Desafio 2

Explique passo a passo como pedir comida por aplicativo.

Tente criar mais de 20 passos.

---

# Resumo do Capítulo

Neste capítulo você aprendeu:

* O que é lógica.
* O que é lógica de programação.
* Como computadores funcionam.
* O que é pensamento computacional.
* O que é um algoritmo.
* Como resolver problemas.
* Os erros mais comuns dos iniciantes.
* Como começar a pensar como programador.
