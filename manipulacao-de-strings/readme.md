# Manipulação de Strings

A manipulação de strings é crucial na programação, permitindo a transformação e análise de texto. Strings são sequências de caracteres e Python fornece uma variedade de métodos para manipulá-las. Este guia detalha métodos importantes e técnicas para trabalhar com strings.

## Métodos de Strings

### `len()`

O método `len()` retorna o número total de caracteres em uma string.

#### Sintaxe

```python
len(string)
```

#### Exemplo básico

```python
texto = "Olá, Mundo!"
tamanho = len(texto)
print(tamanho)  # Resultado: 12
```

### `upper()`

O método `upper()` converte todos os caracteres de uma string para maiúsculas.

#### Sintaxe

```python
string.upper()
```

#### Exemplo básico

```python
texto = "olá, mundo!"
texto_maiusculo = texto.upper()
print(texto_maiusculo)  # Resultado: "OLÁ, MUNDO!"
```

### `lower()`

O método `lower()` converte todos os caracteres de uma string para minúsculas.

#### Sintaxe

```python
string.lower()
```

#### Exemplo básico

```python
texto = "OLÁ, MUNDO!"
texto_minusculo = texto.lower()
print(texto_minusculo)  # Resultado: "olá, mundo!"
```

### `capitalize()`

O método `capitalize()` converte o primeiro caractere da string para maiúsculo e todos os outros caracteres para minúsculo.

#### Sintaxe

```python
string.capitalize()
```

#### Exemplo básico

```python
texto = "olá, mundo!"
texto_capitalizado = texto.capitalize()
print(texto_capitalizado)  # Resultado: "Olá, mundo!"
```

### `find()`

O método `find()` retorna o índice da primeira ocorrência de uma substring. Se a substring não for encontrada, retorna -1.

#### Sintaxe

```python
string.find(substring)
```

#### Exemplo básico

```python
texto = "Olá, Mundo!"
indice = texto.find("Mundo")
print(indice)  # Resultado: 6
```

### `rfind`

O método `rfind()` retorna o índice da última ocorrência de uma substring. Se a substring não for encontrada, retorna -1.

#### Sintaxe

```python
string.rfind(substring)
```

#### Exemplo básico

```python
texto = "Olá, Mundo! Mundo é grande!"
indice = texto.rfind("Mundo")
print(indice)  # Resultado: 15
```

### `split`

O método `split()` divide a string em uma lista de substrings, usando um delimitador especificado.

#### Sintaxe

```python
string.split([delimitador])
```

#### Exemplo básico

```python
texto = "Olá, Mundo! Como vai?"
partes = texto.split(" ")
print(partes)  # Resultado: ['Olá,', 'Mundo!', 'Como', 'vai?']
```

### `join`

O método join() une uma lista de strings em uma única string, usando um delimitador especificado.

#### Sintaxe

```python
delimitador.join(lista_de_strings)
```

#### Exemplo básico

```python
lista = ["Olá", "Mundo", "Como", "vai?"]
texto_unido = " ".join(lista)
print(texto_unido)  # Resultado: "Olá Mundo Como vai?"
```

### `startswith()`

O método `startswith()` retorna True se a string começar com a substring especificada. Caso contrário, retorna False.

#### Sintaxe

```python
string.startswith(substring)
```

#### Exemplo básico

```python
texto = "Python é divertido"
print(texto.startswith("Python"))  # Resultado: True
print(texto.startswith("java"))    # Resultado: False
```

### `endswith()`

O método endswith() retorna True se a string terminar com a substring especificada. Caso contrário, retorna False.

#### Sintaxe

```python
string.endswith(substring)
```

#### Exemplo básico

```python
texto = "Python é divertido"
print(texto.endswith("divertido"))  # Resultado: True
print(texto.endswith("Python"))     # Resultado: False
```

# Concatenar e fatiar strings

## Concatenar Strings

A concatenação de strings é o processo de unir duas ou mais strings em uma só.

#### Sintaxe

```python
string1 + string2
```

#### Exemplo básico

```python
texto1 = "Olá"
texto2 = "Mundo"
texto_concatenado = texto1 + ", " + texto2 + "!"
print(texto_concatenado)  # Resultado: "Olá, Mundo!"
```

## Fatiar Strings

O fatiamento de strings permite extrair partes específicas de uma string.

#### Sintaxe

```python
string[início:fim]
```

#### Exemplo básico

```python
texto = "Python é divertido"
fatia = texto[0:6]
print(fatia)  # Resultado: "Python"
```

A manipulação de strings é uma habilidade essencial para trabalhar com dados textuais em Python. Utilizando os métodos e operações descritos, você pode realizar uma ampla gama de transformações e análises em suas strings. Experimente com diferentes métodos e técnicas para aprimorar suas habilidades em programação e tornar seu trabalho com strings mais eficiente e eficaz.
