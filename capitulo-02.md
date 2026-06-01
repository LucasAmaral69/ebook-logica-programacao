# CAPÍTULO 2 — PENSAMENTO COMPUTACIONAL

## Como Programadores Profissionais Resolvem Problemas

---

# Objetivos do Capítulo

Ao concluir este capítulo, você será capaz de:

* Entender profundamente o conceito de pensamento computacional.
* Aprender os quatro pilares fundamentais.
* Resolver problemas complexos de forma estruturada.
* Desenvolver raciocínio lógico mais avançado.
* Melhorar sua capacidade de criar algoritmos.
* Entender como desenvolvedores experientes pensam.
* Aplicar pensamento computacional fora da programação.
* Começar a construir mentalidade de engenheiro de software.

---

# O Que é Pensamento Computacional?

Muitas pessoas acreditam que programação é aprender código.

Isso está errado.

Código é apenas uma ferramenta.

O verdadeiro diferencial de um programador é a capacidade de resolver problemas.

Essa habilidade é chamada de Pensamento Computacional.

---

## Definição

Pensamento Computacional é uma forma estruturada de analisar problemas, identificar padrões, abstrair informações e criar soluções executáveis. ([FURBOT][1])

---

# Antes do Código Existe o Pensamento

Um erro comum dos iniciantes é abrir o editor e começar a escrever código imediatamente.

Programadores experientes fazem o contrário.

Primeiro eles entendem:

* O problema
* As regras
* Os dados
* As restrições
* Os objetivos

Só depois escrevem código.

---

# Programação é Engenharia de Soluções

Imagine um engenheiro civil.

Ele não começa construindo.

Primeiro ele:

* Analisa terreno
* Calcula estrutura
* Cria projeto

Depois constrói.

Programação funciona exatamente da mesma forma.

---

# A Origem do Pensamento Computacional

O conceito foi popularizado pela cientista da computação Jeannette Wing.

Ela defendia que o pensamento computacional deveria ser uma habilidade básica para qualquer pessoa, assim como leitura e matemática. ([Periódicos UEM][2])

---

# O Grande Objetivo

O pensamento computacional busca responder uma pergunta:

> Como transformar problemas complexos em soluções simples?

---

# Os 4 Pilares do Pensamento Computacional

Segundo os modelos mais difundidos de ensino de computação, o pensamento computacional é sustentado por quatro pilares principais: ([FURBOT][1])

1. Decomposição
2. Reconhecimento de Padrões
3. Abstração
4. Algoritmos

---

# PILAR 1 — DECOMPOSIÇÃO

---

## O Que é Decomposição?

Decomposição é o processo de quebrar um problema grande em problemas menores. ([FURBOT][1])

---

## Por Que Isso é Importante?

O cérebro humano possui limitações.

Quando tentamos resolver tudo ao mesmo tempo:

* Ficamos confusos
* Esquecemos detalhes
* Cometemos erros

Por isso dividimos problemas.

---

# Exemplo Real

Problema:

Criar um sistema para um hospital.

Parece enorme.

---

Mas podemos dividir em:

* Cadastro de pacientes
* Cadastro de médicos
* Consultas
* Exames
* Financeiro
* Estoque de medicamentos

Agora o problema ficou mais controlável.

---

# Exemplo em Programação

Problema:

Criar um aplicativo de delivery.

Divisão:

```text id="a7x4ke"
APP DELIVERY

├── Login
├── Cadastro
├── Restaurantes
├── Carrinho
├── Pagamento
└── Entrega
```

Cada parte pode ser desenvolvida separadamente.

---

# Exemplo do Mundo Real

Imagine que você quer:

"Passar em Engenharia de Software."

Parece algo enorme.

Mas pode ser dividido em:

```text id="x3we8u"
OBJETIVO

Passar na faculdade

↓

Matemática
Programação
Banco de Dados
Redes
Projetos
Provas
```

Você acabou de aplicar decomposição.

---

# Exercício Mental

Problema:

Criar um sistema bancário.

Liste pelo menos:

* 10 subproblemas.

---

# PILAR 2 — RECONHECIMENTO DE PADRÕES

---

## O Que é?

Após dividir um problema, começamos a procurar semelhanças. ([FURBOT][1])

Isso é reconhecimento de padrões.

---

# Exemplo Simples

Observe:

```text id="twdc3f"
2
4
6
8
10
```

Qual o padrão?

Resposta:

+2

---

# Exemplo em Programação

Facebook

Instagram

TikTok

LinkedIn

Todos possuem:

* Login
* Perfil
* Senha
* Usuário

O padrão se repete.

---

# Por Que Isso é Tão Poderoso?

Porque evita reinventar soluções.

Programadores profissionais reutilizam padrões constantemente.

---

# Exemplo Prático

Imagine que você criou:

Sistema de Login.

Depois cria outro projeto.

Você não precisa inventar tudo novamente.

Você reutiliza o padrão.

---

# Design Patterns

Em engenharia de software existem padrões oficiais chamados:

> Design Patterns

São soluções reutilizáveis para problemas recorrentes.

Você aprenderá isso mais adiante.

---

# Exercício

Observe os números:

```text id="yqg7mt"
5
10
20
40
80
```

Qual padrão existe?

---

Resposta:

Multiplicação por 2.

---

# Exercício Avançado

Observe:

```text id="eoh39s"
Login Netflix
Login Spotify
Login Instagram
```

Quais elementos são iguais?

Liste todos.

---

# PILAR 3 — ABSTRAÇÃO

---

# O Pilar Mais Difícil

Muitos iniciantes têm dificuldade aqui.

Abstração significa:

> Focar apenas no que é importante e ignorar o restante. ([FURBOT][1])

---

# Exemplo

Você quer criar um sistema para carros.

Quais dados importam?

* Marca
* Modelo
* Ano
* Placa

---

Quais normalmente não importam?

* Quantidade de poeira
* Nome do antigo dono
* Música tocando no rádio

---

Você ignora o irrelevante.

Isso é abstração.

---

# O Cérebro Faz Isso Constantemente

Quando você olha uma cadeira:

Você não calcula:

* Massa
* Volume
* Quantidade de moléculas

Você apenas entende:

"Cadeira."

Isso é abstração.

---

# Abstração em Programação

Exemplo:

```python id="q6m2bc"
usuario.logar()
```

---

Você não precisa saber:

* Como a senha foi criptografada
* Como o banco funciona
* Como a conexão ocorreu

Você só usa:

```python id="n5v27v"
usuario.logar()
```

A complexidade foi escondida.

---

# Exemplo Profissional

Quando você usa:

```python id="d7q6nq"
print("Olá")
```

Você não sabe como a tela funciona.

Nem precisa.

Isso é abstração.

---

# Exercício

Sistema escolar.

Liste:

O que é importante.

O que pode ser ignorado.

---

# PILAR 4 — ALGORITMOS

---

# O Que é um Algoritmo?

Um algoritmo é uma sequência organizada de passos para resolver um problema. ([FURBOT][1])

---

# Exemplo

Problema:

Atravessar a rua.

---

Algoritmo:

1. Ir até a faixa.
2. Olhar esquerda.
3. Olhar direita.
4. Verificar carros.
5. Atravessar.

---

# Algoritmo Não é Código

Isso é extremamente importante.

Algoritmos existem sem computadores.

---

Exemplo:

Receita de bolo.

É um algoritmo.

---

# Algoritmo Ruim

```text id="3n0v0d"
1. Comer bolo
2. Fazer massa
3. Comprar ingredientes
```

Sem lógica.

---

# Algoritmo Bom

```text id="u1i3qc"
1. Comprar ingredientes
2. Fazer massa
3. Assar
4. Comer
```

---

# Como os 4 Pilares Trabalham Juntos

Imagine:

Criar um aplicativo de transporte.

---

Primeiro:

DECOMPOSIÇÃO

```text id="vlh1c9"
Cadastro
Mapa
Motoristas
Pagamento
Corridas
```

---

Depois:

PADRÕES

```text id="c0n6eg"
Login
Cadastro
Perfil
```

---

Depois:

ABSTRAÇÃO

```text id="3f1oxd"
Importa:

Localização
Motorista
Pagamento

Ignorar:

Cor do celular do usuário
```

---

Depois:

ALGORITMO

```text id="xv0mfa"
Solicitar corrida
Encontrar motorista
Confirmar
Iniciar viagem
Finalizar
Cobrar
```

---

# Como Programadores Sêniores Pensam

Iniciantes:

Pensam em código.

---

Profissionais:

Pensam em sistemas.

---

Iniciantes perguntam:

```text id="f4h7y6"
Como faço um if?
```

---

Profissionais perguntam:

```text id="gh6f1k"
Qual problema preciso resolver?
```

---

Essa diferença muda completamente a carreira.

---

# Pensamento Computacional Fora da Programação

Ele pode ser usado para:

* Estudar melhor
* Organizar finanças
* Criar empresas
* Planejar viagens
* Resolver problemas pessoais

---

# Exemplo Financeiro

Problema:

Você ganha R$ 1400.

Gasta tudo.

Quer economizar.

---

Decomposição:

```text id="e4n7bs"
Alimentação
Transporte
Lazer
Internet
Academia
```

---

Padrões:

```text id="m5r8aw"
Gastos repetidos
```

---

Abstração:

```text id="s7t9po"
Ignorar gastos irrelevantes
Focar nos maiores
```

---

Algoritmo:

```text id="o2v8fg"
Receber salário
Separar despesas
Separar reserva
Gastar restante
```

---

Você acabou de usar pensamento computacional.

---

# Exercícios Práticos

---

## Exercício 1

Quebre o problema abaixo em partes menores:

Criar um sistema de escola.

---

## Exercício 2

Identifique padrões entre:

* Netflix
* YouTube
* Spotify

---

## Exercício 3

Crie uma abstração para:

Sistema de biblioteca.

---

## Exercício 4

Escreva um algoritmo para:

Comprar um produto online.

---

## Exercício 5

Escreva um algoritmo com mais de 20 passos para:

Criar uma conta em rede social.

---

# Desafio de Entrevista Técnica

Problema:

Você precisa criar um sistema de estacionamento.

Antes de programar:

Liste:

* Subproblemas
* Padrões
* Dados importantes
* Algoritmo principal

---

# Erros Comuns

---

## Erro 1

Começar pelo código.

---

## Erro 2

Não entender o problema.

---

## Erro 3

Ignorar planejamento.

---

## Erro 4

Resolver tudo de uma vez.

---

## Erro 5

Não reutilizar soluções.

---

# Resumo do Capítulo

Você aprendeu:

* O que é pensamento computacional.
* Como programadores resolvem problemas.
* Os quatro pilares fundamentais.
* Decomposição.
* Reconhecimento de padrões.
* Abstração.
* Algoritmos.
* Aplicações práticas no mundo real.
* Como pensar mais próximo de um engenheiro de software.
