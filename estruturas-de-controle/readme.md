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

# Operadores lógicos

Os operadores lógicos são usados para combinar múltiplas condições. Em Python, os principais operadores lógicos são `and`, `or` e `not`.

### `and`

O operador and retorna True se ambas as condições forem verdadeiras. Se qualquer uma das condições for falsa, o resultado será False.

#### Sintaxe

```python
condição1 and condição2
```

### Exemplo básico

```python
idade = 20
tem_carteira = True

if idade >= 18 and tem_carteira:
    print("Você pode dirigir.")
else:
    print("Você não pode dirigir.")
```

Neste exemplo, a mensagem "Você pode dirigir." será impressa porque ambas as condições `(idade >= 18` e `tem_carteira)` são verdadeiras.

### `or`

O operador or retorna True se pelo menos uma das condições for verdadeira. Se ambas as condições forem falsas, o resultado será False.

```python
condição1 or condição2
```

### Exemplo básico

```python
chovendo = False
final_de_semana = True

if not chovendo or final_de_semana:
    print("Vamos para o parque!")
else:
    print("Vamos ficar em casa.")
```

Neste exemplo, a mensagem "Vamos para o parque!" será impressa porque pelo menos uma das condições (not chovendo ou final_de_semana) é verdadeira.

### `not`

O operador not inverte o valor lógico da condição. Se a condição for True, not a torna False, e vice-versa.

#### Sintaxe

```python
not condição
```

### Exemplo básico

```python
esta_chovendo = True

if not esta_chovendo:
    print("Vamos sair!")
else:
    print("Vamos ficar em casa.")
```

Neste exemplo, a mensagem "Vamos ficar em casa." será impressa porque a condição (not esta_chovendo) é falsa.
