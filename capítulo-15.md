# CAPÍTULO 15 — ESTRUTURAS DE DADOS

## A Base dos Sistemas Modernos

---

# Objetivos do Capítulo

Ao concluir este capítulo você será capaz de:

* Entender o que são estruturas de dados.
* Compreender por que elas existem.
* Conhecer os principais tipos de estruturas.
* Entender quando utilizar cada estrutura.
* Compreender a relação entre desempenho e organização dos dados.
* Conhecer aplicações reais em sistemas modernos.
* Preparar-se para estudar pilhas, filas, árvores e grafos.

---

# Introdução

Imagine uma biblioteca.

Você possui:

```text
100.000 livros
```

Sem organização:

```text
Caos
```

Com organização:

```text
Corredores

Prateleiras

Categorias

Índices
```

A busca se torna muito mais rápida.

---

Na programação acontece exatamente a mesma coisa.

Os programas precisam armazenar e organizar informações.

É para isso que existem as estruturas de dados.

---

# O Que é uma Estrutura de Dados?

Definição:

> Uma estrutura de dados é uma forma organizada de armazenar, gerenciar e acessar informações na memória.

---

Sem estrutura:

```text
Dados espalhados
```

---

Com estrutura:

```text
Dados organizados
```

---

# Por Que Elas São Importantes?

Imagine um sistema como:

* Netflix
* YouTube
* Instagram
* Spotify
* Banco Digital

Todos precisam armazenar:

* Usuários
* Vídeos
* Mensagens
* Produtos
* Transações

---

Sem estruturas de dados:

```text
Lentidão

Desorganização

Alto consumo de memória
```

---

# Analogia do Mundo Real

Imagine uma gaveta.

---

Sem organização:

```text
Tudo misturado
```

---

Com organização:

```text
Divisórias

Categorias

Separação
```

---

As estruturas de dados funcionam como essas divisórias.

---

# Relação com Algoritmos

Existe uma frase famosa:

> "Algoritmos + Estruturas de Dados = Programas"

---

Algoritmo:

```text
O que fazer
```

---

Estrutura de dados:

```text
Onde guardar
```

---

Exemplo

Aplicativo bancário.

---

Algoritmo:

```text
Transferir dinheiro
```

---

Estrutura:

```text
Armazenar contas
```

---

# Principais Estruturas de Dados

As mais importantes são:

```text
Vetores

Matrizes

Listas

Pilhas

Filas

Árvores

Grafos

Tabelas Hash
```

---

# Visão Geral

```text
Estruturas Lineares

↓

Vetores
Listas
Pilhas
Filas
```

---

```text
Estruturas Não Lineares

↓

Árvores
Grafos
```

---

# Vetores

Já estudamos.

Exemplo:

```python
nomes = [
    "Lucas",
    "Maria",
    "João"
]
```

---

Características:

* Simples
* Rápidos
* Índices fixos

---

Uso comum:

* Listas de produtos
* Notas de alunos
* Dados temporários

---

# Matrizes

Estruturas bidimensionais.

---

Exemplo:

```python
notas = [

    [8, 9],

    [10, 7]

]
```

---

Uso comum:

* Jogos
* Planilhas
* Imagens
* Sistemas científicos

---

# Listas

Semelhantes aos vetores.

Mas possuem maior flexibilidade.

---

Python:

```python
nomes = []

nomes.append("Lucas")
```

---

Permitem:

* Inserção
* Remoção
* Crescimento dinâmico

---

# Pilhas

Funcionam como uma pilha de pratos.

---

Exemplo:

```text
Prato 3

Prato 2

Prato 1
```

---

Sempre removemos o último.

---

Princípio:

```text
LIFO

Last In First Out
```

---

Tradução:

```text
Último que entra

Primeiro que sai
```

---

Aplicações

* Navegadores
* Desfazer (Ctrl + Z)
* Compiladores
* Histórico

---

# Filas

Funcionam como fila de banco.

---

Princípio:

```text
FIFO

First In First Out
```

---

Tradução:

```text
Primeiro que entra

Primeiro que sai
```

---

Exemplo:

```text
Pessoa A

Pessoa B

Pessoa C
```

---

Saída:

```text
Pessoa A
```

---

Aplicações

* Impressoras
* Atendimento
* Sistemas operacionais
* Processamento de tarefas

---

# Árvores

Estrutura hierárquica.

---

Exemplo:

```text
Empresa

↓

Diretor

↓

Gerentes

↓

Funcionários
```

---

Representação:

```text
        A

      /   \

     B     C

   /  \

  D    E
```

---

Aplicações

* Bancos de dados
* Sistemas de arquivos
* Inteligência Artificial
* Buscas rápidas

---

# Grafos

Estrutura utilizada para representar conexões.

---

Exemplo:

```text
Cidade A ---- Cidade B

    |

Cidade C
```

---

Aplicações:

* GPS
* Redes sociais
* Internet
* Rotas de entrega

---

# Tabelas Hash

Uma das estruturas mais importantes da computação.

---

Funcionamento:

```text
Chave

↓

Hash

↓

Posição
```

---

Exemplo Python:

```python
usuario = {

    "nome": "Lucas",

    "idade": 20

}
```

---

Acesso:

```python
print(usuario["nome"])
```

---

Resultado:

```text
Lucas
```

---

Extremamente rápido.

---

# Escolhendo a Estrutura Correta

Pergunta:

```text
Preciso acessar por índice?
```

Use:

```text
Vetor
```

---

Pergunta:

```text
Preciso de inserções frequentes?
```

Use:

```text
Lista
```

---

Pergunta:

```text
Preciso de histórico?
```

Use:

```text
Pilha
```

---

Pergunta:

```text
Preciso processar em ordem?
```

Use:

```text
Fila
```

---

Pergunta:

```text
Preciso de hierarquia?
```

Use:

```text
Árvore
```

---

Pergunta:

```text
Preciso de conexões?
```

Use:

```text
Grafo
```

---

# Estruturas e Desempenho

Um dos maiores erros dos iniciantes:

```text
Ignorar desempenho
```

---

Exemplo

Sistema com:

```text
100 usuários
```

Funciona.

---

Agora:

```text
10 milhões de usuários
```

---

A estrutura escolhida faz enorme diferença.

---

# Caso Real

Instagram.

---

Possui:

* Usuários
* Seguidores
* Curtidas
* Comentários

---

Internamente utiliza:

```text
Grafos

Árvores

Tabelas Hash
```

---

# Caso Real

Google Maps.

---

Possui:

* Cidades
* Ruas
* Distâncias

---

Utiliza:

```text
Grafos
```

---

Para calcular rotas.

---

# Caso Real

Sistema Operacional

---

Gerencia:

* Processos
* Memória
* Arquivos

---

Utiliza:

```text
Filas

Pilhas

Árvores
```

---

# Complexidade

Outro conceito importante.

---

Queremos operações:

```text
Rápidas
```

---

Algumas estruturas são:

```text
Mais rápidas
```

---

Outras:

```text
Mais lentas
```

---

Por isso estudamos algoritmos e estruturas juntos.

---

# Erros Mais Comuns

---

## Erro 1

Usar vetor para tudo.

---

Cada estrutura possui finalidade própria.

---

## Erro 2

Ignorar escalabilidade.

---

Funcionar com:

```text
100 registros
```

não significa funcionar com:

```text
10 milhões
```

---

## Erro 3

Não considerar memória.

---

Estruturas diferentes consomem quantidades diferentes de memória.

---

# Exercícios Resolvidos

---

## Exercício 1

Identifique a estrutura.

Histórico do navegador.

Resposta:

```text
Pilha
```

---

## Exercício 2

Sistema de impressão.

Resposta:

```text
Fila
```

---

## Exercício 3

Sistema de pastas.

Resposta:

```text
Árvore
```

---

# Exercícios 

1. Diferencie vetor e matriz.
2. Explique pilha.
3. Explique fila.
4. Explique árvore.
5. Explique grafo.
6. Cite aplicações de pilhas.
7. Cite aplicações de filas.
8. Cite aplicações de árvores.
9. Cite aplicações de grafos.
10. Cite aplicações de hash.

---

# Desafio

Analise os sistemas abaixo e identifique qual estrutura seria mais adequada:

1. Histórico do navegador.
2. Sistema de impressão.
3. Rede social.
4. GPS.
5. Sistema de arquivos.

Justifique sua resposta.

---

# Curiosidade

Praticamente toda a computação moderna é construída sobre estruturas de dados.

Sem elas não existiriam:

* Bancos digitais.
* Redes sociais.
* Inteligência Artificial.
* Sistemas operacionais.
* Jogos.
* Motores de busca.

---

# Resumo do Capítulo

Você aprendeu:

* O que são estruturas de dados.
* Por que elas existem.
* Vetores.
* Matrizes.
* Listas.
* Pilhas.
* Filas.
* Árvores.
* Grafos.
* Tabelas Hash.
* Aplicações reais.
