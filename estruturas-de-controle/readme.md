# Estruturas de Controle

## Condicionais

As estruturas condicionais são usadas para tomar decisões no seu código com base em certas condições. Em Python, as principais estruturas condicionais são `if`, `else` e `elif`.

### `if`

A instrução `if` avalia uma condição. Se a condição for verdadeira, o bloco de código indentado abaixo do `if` será executado. Se a condição for falsa, o Python ignorará esse bloco de código.

#### Sintaxe

```python
if condição:
    # código a ser executado se a condição for verdadeira
```

### Exemplo básico

```python
idade = 20

if idade >= 18:
    print("Você é maior de idade.") 
```

Neste exemplo, a mensagem "Você é maior de idade." será impressa porque a condição `(idade >= 18)` é verdadeira.

### `else`

A instrução `else` é usada para especificar um bloco de código que será executado se a condição no if for falsa. O else deve vir imediatamente após o bloco de código do if.

#### Sintaxe

```python
if condição:
    # código a ser executado se a condição for verdadeira
else:
    # código a ser executado se a condição for falsa
```

### Exemplo básico

```python
idade = 16

if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
```

Neste exemplo, a mensagem "Você é menor de idade." será impressa porque a condição (idade >= 18) é falsa.

### `elif`

A instrução `elif` (abreviação de "else if") é usada para verificar múltiplas condições. Você pode ter quantos elif precisar entre um if e um else. Se uma das condições elif for verdadeira, o bloco de código correspondente será executado e o restante das condições não será verificado.

#### Sintaxe

```python
if condição1:
    # código a ser executado se a condição1 for verdadeira
elif condição2:
    # código a ser executado se a condição2 for verdadeira
else:
    # código a ser executado se todas as condições acima forem falsas
```

### Exemplo básico

```python
idade = 18

if idade < 18:
    print("Você é menor de idade.")
elif idade == 18:
    print("Você tem exatamente 18 anos.")
else:
    print("Você é maior de idade.")
```

Neste exemplo, a mensagem "Você tem exatamente 18 anos." será impressa porque a condição (idade == 18) é verdadeira.
