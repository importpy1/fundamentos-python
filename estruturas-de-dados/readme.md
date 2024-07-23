# Estruturas de Dados

As estruturas de dados em Python permitem armazenar e manipular diferentes tipos de dados de forma eficiente. Neste documento, abordaremos quatro principais estruturas de dados: Listas, Tuplas, Dicionários e Conjuntos. Cada uma delas tem suas próprias características e métodos úteis para o desenvolvimento em Python.

## Listas

Listas são coleções ordenadas e mutáveis de itens, que podem ser de diferentes tipos. Elas são uma das estruturas de dados mais versáteis em Python.

#### Declaração

Você pode declarar uma lista usando colchetes `[]` e separando os itens por vírgulas.

#### Sintaxe

```python
lista = [item1, item2, item3]
```
#### Exemplo básico

```python
frutas = ["maçã", "banana", "laranja"]
```

#### Indexação

Os itens em uma lista são indexados a partir do índice 0. Você pode acessar um item da lista usando seu índice.

```python
item = lista[indice]
```

#### Exemplo

```python
primeira_fruta = frutas[0]  # Resultado: "maçã"
segunda_fruta = frutas[1] # "banana"
terceira_fruta = fruta[2] # "laranja"
```

### Métodos básicos

### `append(item)`

Adiciona um item ao final da lista.

#### Sintaxe

```python
lista.append(item)
```

#### Exemplo básico

```python
frutas.append("uva")
print(frutas)  # Resultado: ["maçã", "banana", "laranja", "uva"]
```

### `remove(item)`

Remove o primeiro item com o valor especificado.

#### Sintaxe

```python
lista.remove(item)
```

#### Exemplo básico

```python
frutas.remove("banana")
print(frutas)  # Resultado: ["maçã", "laranja", "uva"]
```

