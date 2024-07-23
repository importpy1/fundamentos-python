# Estruturas de Repetição

As estruturas de repetição, ou loops, são usadas para executar um bloco de código várias vezes. Em Python, as principais estruturas de repetição são `for` e `while`.

### `for`

O loop `for` é usado para iterar sobre uma sequência (como uma lista, tupla, dicionário, conjunto ou string) ou outros objetos iteráveis.

#### Sintaxe

```python
for item in sequência:
    # código a ser executado para cada item na sequência
```

### Exemplo básico

```python
frutas = ["maçã", "banana", "cereja"]

for fruta in frutas:
    print(fruta)

# Saída:

maçã
banana
cereja
```

Neste exemplo, o loop for iterará sobre a lista frutas e imprimirá cada fruta.

### `while`

O loop while é usado para repetir um bloco de código enquanto uma condição é verdadeira. O loop continuará executando enquanto a condição permanecer verdadeira.

#### Sintaxe

```python
while condição:
    # código a ser executado enquanto a condição for verdadeira
```

### Exemplo básico

```python
contador = 0

while contador < 5:
    print(contador)
    contador += 1
```

Neste exemplo, o loop while continuará executando enquanto a variável contador for menor que 5. A cada iteração, contador é incrementado em 1 até que a condição se torne falsa.
