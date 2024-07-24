# Fundamentos básicos

## Variáveis e Tipos Primitivos

### O que são Variáveis?

Variáveis são como caixas onde você pode armazenar diferentes tipos de dados. Você dá um nome à caixa e pode colocar (ou atualizar) valores nela ao longo do tempo. Em Python, você não precisa declarar o tipo da variável explicitamente; o tipo é inferido pelo valor atribuído.

```python
numero = 10

# Acima, `numero` é nossa variável e 10 é o valor atribuído a ela
```


### Tipos primitivos

Os tipos primitivos são os tipos de dados mais básicos em uma linguagem de programação. Em Python, os principais tipos primitivos são:

- Inteiros (`int`): Números inteiros sem parte decimal.

```python
idade = 25
ano_atual = 2024
```

- Floats (`float`): Números com parte decimal.

```python
altura = 1.81
preco = 20.99
```

- Strings (`string`): Sequências de caracteres, usadas para representar texto.

```python
nome = "Cléber"
texto = "Isso aqui é uma string"
```

- Booleanos (`bool`): Valores lógicos que podem ser True (verdadeiro) ou False (falso).

```python
ativo = True
aposentado = False
```

## Operadores aritméticos

### Para que servem os operadores aritméticos

Os operadores aritméticos são usados para realizar operações matemáticas básicas. Em Python, você pode usar os seguintes operadores:

- Adição (`+`): Realiza a soma de números

```python
soma = 10 + 5 # Resultado: 15
```


- Subtração (`-`): Subtrai um número do outro

```python
diferenca = 10 - 5  # Resultado: 5 
```


- Multiplicação (`*`): Multiplica dois números

```python
produto = 10 * 5 # Resultado: 50 
```


- Divisão (`/`): Divide um número pelo outro, resultando em um número float.

```python
divisao = 10 / 5 # Resultado 2.0 
```


- Divisão inteira (`//`): Divide um número pelo outro, resultando no quociente inteiro da divisão.

```python
divisao_inteira = 10 // 3  # Resultado: 3
```


- Módulo (`%`): Retorna o resto da divisão de um número pelo outro.

```python
resto = 10 % 3 # Resultado: 1
```

## Entrada e Saída (input e print)

#### Entrada (`input`)

A função `input()` é usada para receber dados do usuário. Ela sempre retorna uma string, então você pode precisar converter a string para outro tipo de dado, se necessário.

```python
nome = input("Qual é o seu nome? ")
idade = int(input("Quantos anos você tem? "))
```

#### Saída (`print()`)

A função `print()` é usada para exibir dados na tela.

```python
print("Olá, Mundo!")
print("Meu nome é", nome)
print("Eu tenho", idade, "anos")
```

#### Exemplos

```python
# Entrada de dados
nome = input("Digite seu nome: ")
idade = int(input("Digite sua idade: "))
altura = float(input("Digite sua altura: "))

# Saída de dados
print(f"Nome: {nome}")
print(f"Idade: {idade}")
print(f"Altura: {altura}")

```

Com esses fundamentos básicos, você está pronto para começar a explorar o mundo da programação em Python. Pratique criando suas próprias variáveis, usando operadores aritméticos e interagindo com o usuário através de entrada e saída de dados!
