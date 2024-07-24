# Funções em Python

Funções são blocos de código reutilizáveis que realizam uma tarefa específica. Elas ajudam a tornar o código mais modular, organizado e fácil de manter.

## Declaração e Chamada de Funções

### Declaração

Para declarar uma função, utiliza-se a palavra-chave `def`, seguida pelo nome da função, parênteses e dois pontos. O corpo da função é indentado.

#### Sintaxe

```python
def nome_da_funcao(parametros):
    # corpo da função
    pass
```

#### Exemplo básico

```python
def saudacao():
    print("Olá, mundo!")
```

#### Chamada de Função

Para chamar uma função, basta usar seu nome seguido de parênteses.

```python
saudacao()  # Saída: Olá, mundo!
```

## Argumentos e Parâmetros

Funções podem aceitar valores chamados argumentos, que são passados para os parâmetros da função.

#### Exemplo com argumentos

```python
def saudacao(nome):
    print(f"Olá, {nome}!")

saudacao("Alice")  # Saída: Olá, Alice!
```

### Argumentos padrão

Parâmetros podem ter valores padrão, que são usados se nenhum argumento for passado.

```python
def saudacao(nome="mundo"):
    print(f"Olá, {nome}!")

saudacao()       # Saída: Olá, mundo!
saudacao("Bob")  # Saída: Olá, Bob!
```

### Argumentos nomeados

Você pode passar argumentos para uma função usando o nome dos parâmetros.

#### Exemplo básico

```python
def saudacao(nome, saudacao="Olá"):
    print(f"{saudacao}, {nome}!")

saudacao(nome="Alice", saudacao="Oi")  # Saída: Oi, Alice!
```

### Número Variável de Argumentos
Você pode definir funções que aceitam um número variável de argumentos usando *args e **kwargs.

### `*args`

Permite passar um número variável de argumentos posicionais para uma função.

### Exemplo básico

```python
def soma(*numeros):
    total = 0
    for numero in numeros:
        total += numero
    return total

print(soma(1, 2, 3))  # Saída: 6
```

### `kwargs`

Permite passar um número variável de argumentos nomeados para uma função.

```python
def detalhes_usuario(**kwargs):
    for chave, valor in kwargs.items():
        print(f"{chave}: {valor}")

detalhes_usuario(nome="Alice", idade=30, cidade="São Paulo")
# Saída:
# nome: Alice
# idade: 30
# cidade: São Paulo
```

## Funções com retorno

Funções podem retornar valores utilizando a palavra-chave `return`.

#### Exemplo básico

```python
def soma(a, b):
    return a + b

resultado = soma(3, 4)
print(resultado)  # Saída: 7
```

### Retornando múltiplos valores

Funções podem retornar múltiplos valores como uma tupla.

#### Exemplo básico

```python
def operacoes(a, b):
    soma = a + b
    diferenca = a - b
    return soma, diferenca

resultado_soma, resultado_diferenca = operacoes(10, 5)
print(resultado_soma)       # Saída: 15
print(resultado_diferenca)  # Saída: 5
```

## Funções lambdas

Funções lambda são funções anônimas, definidas utilizando a palavra-chave `lambda`. Elas são geralmente usadas para funções simples e de curta duração.

#### Sintaxe

```python
lambda argumentos: expressão
```

#### Exemplo básico

```python
soma = lambda a, b: a + b
print(soma(3, 4))  # Saída: 7
```

## Documentação de funções

Funções podem (e devem) ser documentadas utilizando docstrings. Docstrings são strings que descrevem a função e são colocadas logo após a declaração da função.

#### Exemplo básico

```python
def saudacao(nome):
    """
    Esta função imprime uma saudação com o nome fornecido.
    
    Parâmetros:
    nome (str): O nome da pessoa a ser saudada.
    """
    print(f"Olá, {nome}!")

saudacao("Alice")
```

## Conclusão
Funções são uma parte fundamental da programação em Python, permitindo a criação de código modular e reutilizável. Entender como declarar, chamar e utilizar funções eficientemente é essencial para qualquer desenvolvedor Python. Pratique a criação e uso de funções para melhorar sua habilidade de escrever código limpo e organizado. Funções também permitem a abstração de lógica complexa em blocos de código gerenciáveis, tornando seu desenvolvimento mais ágil e estruturado.
