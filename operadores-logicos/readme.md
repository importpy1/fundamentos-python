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
