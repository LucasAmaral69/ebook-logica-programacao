# CAPÍTULO 5 — FLUXOGRAMAS

## Transformando Algoritmos em Diagramas Visuais

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que é um fluxograma.
* Compreender a importância dos diagramas na programação.
* Conhecer os símbolos oficiais.
* Criar fluxogramas simples e complexos.
* Transformar problemas em representações visuais.
* Identificar erros lógicos antes da programação.
* Ler fluxogramas profissionais.
* Converter fluxogramas em algoritmos e código.

---

# Introdução

Até agora aprendemos:

* Pensamento Computacional
* Resolução de Problemas
* Algoritmos

Mas existe um problema.

Muitas vezes um algoritmo escrito apenas em texto pode ser difícil de visualizar.

Observe:

```text
1. Ler idade
2. Verificar idade
3. Se idade ≥ 18
      Mostrar "Maior"
4. Senão
      Mostrar "Menor"
5. Encerrar
```

Conseguimos entender.

Mas e se o algoritmo tiver:

* 50 passos?
* 100 decisões?
* Várias repetições?

Fica difícil.

Foi por isso que surgiram os fluxogramas.

---

# O Que é um Fluxograma?

Um fluxograma é uma representação gráfica de um algoritmo.

Em vez de escrever apenas texto, utilizamos símbolos conectados por setas.

Esses símbolos representam:

* Início
* Processos
* Entradas
* Saídas
* Decisões
* Fim

---

# Por Que Fluxogramas Existem?

Fluxogramas ajudam a:

* Visualizar problemas.
* Planejar sistemas.
* Encontrar erros.
* Explicar processos.
* Documentar programas.

---

# Onde São Utilizados?

Fluxogramas não são usados apenas em programação.

Também aparecem em:

* Empresas
* Engenharia
* Medicina
* Indústrias
* Bancos
* Hospitais

---

# Exemplo Real

Imagine um caixa eletrônico.

Quando você realiza um saque:

```text
Inserir cartão
↓
Digitar senha
↓
Senha correta?
↓
Sim → Continuar
Não → Bloquear acesso
```

Isso é um fluxo.

Pode ser representado por um fluxograma.

---

# Os Símbolos Oficiais

Existem diversos símbolos.

Porém alguns são muito mais utilizados.

---

# 1. Terminador (Início/Fim)

Representa:

* Início
* Encerramento

Formato:

```text
╭──────────╮
│ INÍCIO   │
╰──────────╯
```

ou

```text
╭──────────╮
│ FIM      │
╰──────────╯
```

---

# 2. Processo

Representa uma ação.

Formato:

```text
┌─────────────┐
│ PROCESSO    │
└─────────────┘
```

Exemplos:

* Somar números
* Calcular média
* Atualizar saldo

---

# 3. Entrada e Saída

Representa leitura ou exibição de dados.

Formato:

```text
╱──────────╲
╲──────────╱
```

Exemplos:

* Ler nome
* Ler idade
* Mostrar resultado

---

# 4. Decisão

Representa uma pergunta.

Formato:

```text
      ◇
```

Exemplos:

* Idade ≥ 18?
* Senha correta?
* Saldo suficiente?

---

# 5. Setas

Representam direção.

```text
↓
↑
→
←
```

Sem as setas não existe fluxo.

---

# Exemplo Completo

Problema:

Exibir mensagem de boas-vindas.

---

Algoritmo:

```text
1. Iniciar
2. Mostrar "Bem-vindo"
3. Encerrar
```

---

Fluxograma:

```text
╭────────╮
│ INÍCIO │
╰────────╯
     ↓

╱────────────╲
╲ Bem-vindo! ╱

     ↓

╭──────╮
│ FIM  │
╰──────╯
```

---

# Fluxogramas com Decisão

Agora vamos criar algo mais interessante.

---

Problema

Verificar maioridade.

---

Algoritmo

```text
Ler idade

Se idade >= 18
      Mostrar "Maior"

Senão
      Mostrar "Menor"

Fim
```

---

Fluxograma

```text
INÍCIO
   ↓

LER IDADE
   ↓

IDADE >= 18 ?

↙         ↘

SIM       NÃO

↓          ↓

MAIOR     MENOR

↓          ↓

    FIM
```

---

# Estudo de Caso 1

Sistema de Login

---

Passos:

```text
1. Ler usuário
2. Ler senha
3. Verificar senha
4. Permitir acesso
```

---

Fluxograma

```text
INÍCIO
   ↓

LER USUÁRIO
   ↓

LER SENHA
   ↓

SENHA CORRETA?

↙         ↘

SIM       NÃO

↓          ↓

ENTRAR    ERRO

↓          ↓

    FIM
```

---

# Estudo de Caso 2

Sistema de Notas

---

Problema:

Aprovar aluno.

Regra:

Média ≥ 7

---

Fluxograma:

```text
INÍCIO
   ↓

LER NOTA 1
   ↓

LER NOTA 2
   ↓

CALCULAR MÉDIA
   ↓

MÉDIA >= 7 ?

↙         ↘

SIM       NÃO

↓          ↓

APROVADO REPROVADO

↓          ↓

    FIM
```

---

# Fluxogramas e Loops

Fluxogramas também podem representar repetições.

---

Problema:

Contar de 1 até 5.

---

Fluxo:

```text
INÍCIO
   ↓

CONTADOR = 1
   ↓

CONTADOR <= 5 ?

↙         ↘

SIM       NÃO

↓          ↓

MOSTRAR    FIM

↓
CONTADOR++

↓
VOLTAR
```

---

# Como Ler um Fluxograma

Sempre siga as setas.

---

Exemplo:

```text
INÍCIO

↓

LER IDADE

↓

IDADE >= 18?
```

Quando chegar em uma decisão:

Escolha o caminho correto.

---

# Erros Comuns

---

## Erro 1

Não colocar início.

---

Errado:

```text
Ler idade
↓
Mostrar idade
```

---

Correto:

```text
INÍCIO
↓
Ler idade
↓
Mostrar idade
↓
FIM
```

---

# Erro 2

Fluxo sem direção.

---

Errado:

```text
Ler idade

Mostrar idade

Fim
```

---

Sem setas.

Sem fluxo.

---

# Erro 3

Múltiplas ações na mesma caixa.

---

Ruim:

```text
Ler nome
Calcular idade
Mostrar resultado
```

---

Melhor:

```text
Ler nome

↓

Calcular idade

↓

Mostrar resultado
```

---

# Erro 4

Decisões mal definidas.

---

Ruim:

```text
Está certo?
```

---

Bom:

```text
Média >= 7 ?
```

---

# Fluxogramas em Empresas

Antes de sistemas serem desenvolvidos, muitas empresas desenham fluxogramas para:

* Aprovação de processos
* Sistemas bancários
* Sistemas hospitalares
* Sistemas de pagamento

Isso reduz erros.

---

# Exemplo Profissional

Compra online.

Fluxo simplificado:

```text
Selecionar produto

↓

Adicionar carrinho

↓

Realizar pagamento

↓

Pagamento aprovado?

↙            ↘

SIM          NÃO

↓             ↓

Enviar      Tentar
pedido      novamente

↓

Fim
```

---

# Transformando Fluxograma em Algoritmo

Fluxograma:

```text
Ler nota

↓

Nota >= 60?

↓

Aprovado
```

---

Algoritmo:

```text
1. Ler nota

2. Se nota >= 60
      Mostrar aprovado

3. Fim
```

---

# Transformando Algoritmo em Fluxograma

Algoritmo:

```text
1. Ler salário

2. Calcular bônus

3. Mostrar salário final
```

---

Fluxograma:

```text
INÍCIO

↓

LER SALÁRIO

↓

CALCULAR BÔNUS

↓

MOSTRAR RESULTADO

↓

FIM
```

---

# Ferramentas Para Criar Fluxogramas

## Gratuitas

* [Draw.io (diagrams.net)](https://app.diagrams.net/?utm_source=chatgpt.com)
* [Lucidchart](https://www.lucidchart.com/?utm_source=chatgpt.com)
* [Canva](https://www.canva.com/?utm_source=chatgpt.com)
* [Miro](https://miro.com/?utm_source=chatgpt.com)

---

# Exercício Resolvido

Problema:

Verificar se um número é positivo.

---

Fluxograma:

```text
INÍCIO

↓

LER NÚMERO

↓

NÚMERO > 0 ?

↙         ↘

SIM       NÃO

↓          ↓

POSITIVO  NÃO POSITIVO

↓

FIM
```

---

# Exercícios


1. Fluxograma para somar dois números.
2. Fluxograma para calcular média.
3. Fluxograma para converter metros em centímetros.
4. Fluxograma para calcular idade.
5. Fluxograma para calcular área de um quadrado.
6. Fluxograma para verificar aprovação.
7. Fluxograma para verificar número par.
8. Fluxograma para calcular desconto.
9. Fluxograma para validar senha.
10. Fluxograma para verificar saldo bancário.


# Desafio

Crie um fluxograma completo para um sistema de estacionamento.

Requisitos:

* Entrada do veículo.
* Registro de horário.
* Cálculo de permanência.
* Cálculo de valor.
* Pagamento.
* Saída.

---

# Resumo do Capítulo

Você aprendeu:

* O que é um fluxograma.
* Por que fluxogramas são importantes.
* Os símbolos fundamentais.
* Como representar decisões.
* Como representar repetições.
* Como converter algoritmos em fluxogramas.
* Como converter fluxogramas em algoritmos.
* Ferramentas profissionais para criar diagramas.
