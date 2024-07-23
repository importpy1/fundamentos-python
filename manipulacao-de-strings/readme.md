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

O método upper() converte todos os caracteres de uma string para maiúsculas.

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

O método lower() converte todos os caracteres de uma string para minúsculas.

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

O método capitalize() converte o primeiro caractere da string para maiúsculo e todos os outros caracteres para minúsculo.

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

