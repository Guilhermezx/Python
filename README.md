# Python

## Diferença de Lista do Python e Array do NumPy

```python
import pandas as pd
import numpy as np

num_elementos = 100

# Lista de Elementos utilizando o Python

#lista_elementos = []
#for x in range (num_elementos):
#lista_elementos.append(x)
#print(lista_elementos[-1])

#Lista de Elementos utilizando o Array do NumPy
array_elementos = np.arange(num_elementos)
print(array_elementos[-1])
```

# # Criação de Array no NumPy
```python
import numpy as np

array_teste = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])

print(f"Criação de Array no NumPy utilizando o metodo .array:\n{array_teste}\n") # mostra o conteúdo dentro do array_teste.
print(f"Criação de Array no NumPy utilizando o metodo .ones:\n{np.ones([20])}\n") # Cria uma quantidade determinada de numeros 1, a quantidade é definida dentro do [].
print(f"Criação de Array no NumPy utilizando o metodo .zeros:\n{np.zeros([20])}\n") # Cria uma quantidade determinada de numeros 0, a quantidade é definida dentro do [].
print(f"Criação de Array no NumPy utilizando o metodo .Empty:\n{np.empty([15])}\n") # Cria um novo Array sem inicializar seus valores, o conteudo da array sera um bloco de memoria não inicializado.
print(f"Criação de Array no NumPy utilizando o metodo .arange:\n{np.arange(20)}\n") # Cria um Array contendo uma sequencia de valores, que retorna uma array em vez de uma lista.
print(f"Criação de Array no NumPy utilizando o metodo .Linspace:\n{np.linspace(0, 40, num = 41)}\n") #Cria uma Array determinando o inicio de o fim, e também espaçamentos.
```

# # NumPy: A importancia de Definir o tipo de dados
```python
import numpy as np

num_elementos = 1000000000

array_perfomance = np.zeros(num_elementos, dtype = np.int8)
#dtype é um parametro que define o tipo  de dados dos elementos que estão dentro da Array
#int8 significa que os elementos deste array criado será um inteiro de 8bits, variando entre (-128 a 127)
# Isto define e ajuda a velocidade que o codigo vai ser executado.
```

# # Criação de numeros Randomicos
```python
import numpy as np

rng = np.random.default_rng() # Cria uma instância no gerador de numeros aleatorios
print(rng.random(10)) # Gera e imprime os numeros aleatorios, no caso sera gerado 10 numeros de ponto flutuante, sempre que o codigo for executado.


#Para iniciar a aleatoriedade a partir de um numero especifido:

array_aleatorio = rng.uniform(2, 15, 3) # Vai ser gerado um Array aleatorio a partir de um numero espeficido.
print(array_aleatorio)

# 2 = O Menor numero que o array pode chegar.
# 15 = O Maior numero que o Array pode chegar.
# 3 = A Quantidade de numeros aleatorio que vão ser gerado.
```