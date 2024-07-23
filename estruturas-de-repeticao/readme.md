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

## Usando range() com for

O método range() gera uma sequência de números, que pode ser usada para controlar a quantidade de iterações em um loop for.

#### Sintaxe

```python
range(início, fim, passo)
```

- início (opcional): O valor inicial da sequência. O padrão é 0.
- fim: O valor final da sequência (não incluído na sequência).
- passo (opcional): O valor a ser adicionado a cada iteração. O padrão é 1.

#### Exemplo básico

```python
for i in range(5):
    print(i)
```

Neste exemplo, range(5) gera uma sequência de números de 0 a 4. O loop for imprime cada número dessa sequência.

#### Exemplo avançado com range()

```python
for i in range(2, 10, 2):
    print(i)
```

Neste exemplo, range(2, 10, 2) gera uma sequência de números começando em 2, indo até 10 (não incluído) e avançando de 2 em 2. O loop for imprime os números 2, 4, 6 e 8.

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

# Saída:

0
1
2
3
4

```

Neste exemplo, o loop while continuará executando enquanto a variável contador for menor que 5. A cada iteração, contador é incrementado em 1 até que a condição se torne falsa.

# Break e Continue

As instruções break e continue são usadas para controlar o fluxo dos loops.

### `break`

A instrução break é usada para encerrar um loop prematuramente. Quando o break é encontrado dentro de um loop, o loop é imediatamente encerrado e o controle do programa passa para a próxima instrução após o loop.

#### Sintaxe

```python
for item in sequência:
    if condição:
        break
    # código a ser executado

```

### Exemplo básico

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

Neste exemplo, o loop for é interrompido quando i é igual a 5, então apenas os números de 0 a 4 são impressos.

### `continue`

A instrução continue é usada para pular a iteração atual do loop e continuar com a próxima iteração. Quando o continue é encontrado dentro de um loop, o loop pula o restante do seu corpo e reinicia na próxima iteração.

#### Sintaxe

```python
for item in sequência:
    if condição:
        continue
    # código a ser executado
```

### Exemplo básico

```python
for i in range(10):
    if i % 2 == 0:
        continue
    print(i)
```

Neste exemplo, o continue faz com que o loop pule a impressão dos números pares e continue com a próxima iteração. Apenas os números ímpares de 0 a 9 são impressos.
