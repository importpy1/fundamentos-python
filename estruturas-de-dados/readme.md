# Estruturas de Dados

As estruturas de dados em Python permitem armazenar e manipular diferentes tipos de dados de forma eficiente. Neste documento, abordaremos quatro principais estruturas de dados: Listas, Tuplas e Dicionários. Cada uma delas tem suas próprias características e métodos úteis para o desenvolvimento em Python.

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

### `pop(indice)`

Remove e retorna o item no índice especificado.

#### Sintaxe

```python
item = lista.pop(indice)
```

#### Exemplo básico

```python
ultima_fruta = frutas.pop()
print(ultima_fruta)  # Resultado: "uva"
print(frutas)        # Resultado: ["maçã", "laranja"]
```

### `sort()`

Ordena os itens da lista

#### Sintaxe

```python
lista.sort()
```

#### Exemplo básico

```python
frutas.sort()
print(frutas)  # Resultado: ["laranja", "maçã", "manga", "pera"]
```

### `extend(outra_lista)`

Adiciona todos os itens de outra lista à lista atual.

#### Sintaxe

```python
lista.extend(outra_lista)
```

#### Exemplo básico

```python
frutas.extend(["pera", "manga"])
print(frutas)  # Resultado: ["maçã", "laranja", "pera", "manga"]
```

## Tuplas

Tuplas são coleções ordenadas e imutáveis de itens. Uma vez criada, uma tupla não pode ser alterada.

#### Declaração

Você pode declarar uma tupla usando parênteses `()` e separando os itens por vírgulas.

#### Sintaxe

```python
tupla = (item1, item2, item3)
```

#### Exemplo básico

```python
coordenadas = (10, 20)
```
### Características das Tuplas

- Imutabilidade: Uma vez que uma tupla é criada, seus valores não podem ser alterados.
- Ordenadas: Os itens em uma tupla têm uma ordem definida e essa ordem não muda.
- Heterogêneas: Tuplas podem conter itens de diferentes tipos de dados.

### Acessando tuplas

Os itens em uma tupla podem ser acessados usando indexação, semelhante a listas.

#### Sintaxe

```python
item = tupla[indice]
```

#### Exemplo básico

```python
coordenadas = (10, 20)
x = coordenadas[0]  # Resultado: 10
y = coordenadas[1]  # Resultado: 20
```

### Métodos básicos

Embora tuplas sejam imutáveis, existem algumas operações e métodos que podem ser usados com elas.

### `count()`

O método `count()` retorna o número de vezes que um valor especificado aparece na tupla.

#### Sintaxe

```python
tupla.count(item)
```

#### Exemplo básico

```python
numeros = (1, 2, 2, 3, 4, 2, 5)
contagem = numeros.count(2)
print(contagem)  # Resultado: 3
```

### `index()`

O método `index()` retorna o índice da primeira ocorrência de um valor especificado.

#### Sintaxe

```python
tupla.index(item)
```

#### Exemplo básico

```python
frutas = ("maçã", "banana", "laranja")
indice = frutas.index("banana")
print(indice)  # Resultado: 1
```

### `sum()`

A função `sum()` retorna a soma dos itens em uma tupla de números.

#### Sintaxe

```python
sum(tupla)
```

#### Exemplo

```python
numeros = (1, 2, 3, 4, 5)
soma = sum(numeros)
print(soma)  # Resultado: 15
```

### `min()` e `max()`

As funções min() e max() retornam o menor e o maior item em uma tupla, respectivamente.

#### Sintaxe

```python
min(tupla)
max(tupla)
```

#### Exemplo básico

```python
numeros = (1, 2, 3, 4, 5)
menor = min(numeros)
maior = max(numeros)
print(menor)  # Resultado: 1
print(maior)  # Resultado: 5
```

## Dicionários

Dicionários são estruturas de dados que armazenam pares chave-valor. Eles são úteis para armazenar dados que precisam ser associados e permitem acesso rápido aos valores correspondentes às suas chaves.

#### Declaração

Dicionários são declarados usando chaves `{}` e pares chave-valor são separados por dois pontos `:`.

#### Sintaxe

```python
dicionario = {
    'chave1': 'valor1',
    'chave2': 'valor2',
    'chave3': 'valor3'
}
```

#### Exemplo básico

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
```

### Acessando valores

Os valores em um dicionário podem ser acessados usando suas chaves.

#### Sintaxe

```python
valor = dicionario['chave']
```

#### Exemplo básico

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
nome = pessoa['nome']  # Resultado: 'João'
```

### Adicionando e atualizando itens

Itens podem ser adicionados ou atualizados em um dicionário usando a sintaxe de atribuição.

#### Sintaxe

```python
dicionario['nova_chave'] = 'novo_valor'
dicionario['chave_existente'] = 'valor_atualizado'
```

#### Exemplo básico

```python
pessoa = {
    'nome': 'João',
    'idade': 25
}
pessoa['cidade'] = 'São Paulo'  # Adicionando nova chave-valor
pessoa['idade'] = 26            # Atualizando valor existente
```

### Removendo itens

Itens podem ser removidos de um dicionário usando o método `pop()` ou a palavra-chave `del`.

#### Sintaxe

```python
dicionario.pop('chave')
del dicionario['chave']
```

#### Exemplo básico

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
pessoa.pop('idade')    # Remove a chave 'idade'
del pessoa['cidade']   # Remove a chave 'cidade'
```

### Métodos básicos

### `keys()`

O método `keys()` retorna uma visualização das chaves no dicionário.

#### Sintaxe

```python
dicionario.keys()
```

#### Exemplo básico

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
chaves = pessoa.keys()
print(chaves)  # Resultado: dict_keys(['nome', 'idade', 'cidade'])
```

### `values()`

O método `values()` retorna uma visualização dos valores no dicionário.

#### Sintaxe

```python
dicionario.values()
```

#### Exemplo básico

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
valores = pessoa.values()
print(valores)  # Resultado: dict_values(['João', 25, 'São Paulo'])
```

### `items()`

O método `items()` retorna uma visualização dos pares chave-valor no dicionário.

#### Sintaxe

```python
dicionario.items()
```

#### Exemplo básico

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
itens = pessoa.items()
print(itens)  # Resultado: dict_items([('nome', 'João'), ('idade', 25), ('cidade', 'São Paulo')])
````

### `get()`

O método `get()` retorna o valor para uma chave especificada. Se a chave não existir, retorna um valor padrão (None, por padrão).

#### Sintaxe

```python
dicionario.get('chave', valor_padrao)
```

#### Exemplo básico

```python
pessoa = {
    'nome': 'João',
    'idade': 25
}
idade = pessoa.get('idade', 0)        # Resultado: 25
cidade = pessoa.get('cidade', 'N/A')  # Resultado: 'N/A'
```

### `update()`

O método `update()` atualiza o dicionário com os pares chave-valor de outro dicionário.

#### Sintaxe

```python
dicionario.update(outro_dicionario)
```

#### Exemplo básico

```python
pessoa = {
    'nome': 'João',
    'idade': 25
}
pessoa.update({'cidade': 'São Paulo', 'idade': 26})
print(pessoa)  # Resultado: {'nome': 'João', 'idade': 26, 'cidade': 'São Paulo'}
```

### `clear()`

O método `clear()` remove todos os itens do dicionário.

#### Sintaxe

```python
dicionario.clear()
```

#### Exemplo básico 

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
pessoa.clear()
print(pessoa)  # Resultado: {}
```

### Iterando sobre um dicionário

#### Iterando sobre `chaves`

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
for chave in pessoa.keys():
    print(chave)
```

#### Iterando sobre `valores`

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
for valor in pessoa.values():
    print(valor)
```

#### Iterando sobre `pares chave-valor`

```python
pessoa = {
    'nome': 'João',
    'idade': 25,
    'cidade': 'São Paulo'
}
for chave, valor in pessoa.items():
    print(f"{chave}: {valor}")
```

## Conclusão

Estruturas de dados são fundamentais em Python, permitindo armazenar e manipular conjuntos de dados de maneira eficiente. Listas, tuplas, dicionários e conjuntos cada um possui características e usos específicos:

- **Listas** são mutáveis e ideais para coleções ordenadas.
- **Tuplas** são imutáveis e úteis para armazenar dados constantes.
- **Dicionários** utilizam pares chave-valor para associações rápidas.

Compreender e utilizar essas estruturas de dados de forma eficaz pode melhorar significativamente a eficiência e a clareza do seu código. A prática com cada uma delas permitirá escolher a estrutura mais adequada para cada situação, resultando em soluções mais elegantes e performáticas.
