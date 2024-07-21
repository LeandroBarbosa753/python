# Introdução ao Python

Este notebook é uma introdução prática à linguagem Python, cobrindo conceitos básicos e intermediários, incluindo variáveis, operadores aritméticos, estruturas de controle de fluxo, listas, dicionários, tuplas, e mais. O objetivo é fornecer uma base sólida para o desenvolvimento em Python através de exemplos e exercícios práticos.

## Links e Recursos

- **Google Colab**: [Acesso ao Google Colab](https://colab.research.google.com/drive/1bHP0BICqNOHGTocwyZKwz5C2hKP7ILPO?authuser=1)

## Sumário

1. Introdução
2. Comentários em Python
3. Variáveis
    - Tipos de Variáveis
    - Strings
    - Números
4. Operadores Aritméticos
5. Identação
6. Entrada de Comandos
7. Exercícios
8. Casting
9. Manipulação de Strings
    - Invertendo Strings
    - Testando a Existência de Caracteres
    - Imutabilidade
    - Métodos
10. Formatação de Strings
11. Comandos de Decisão
12. Laços de Repetição
    - While
    - For
13. Listas
14. Conjuntos (Sets)
15. Tuplas
16. Dicionários
17. Lista Comprehensions
18. Funções
    - Exemplo de Definição de Função
    - Função que "não faz nada"
    - Parâmetros em Função
    - Exemplo de Soma
    - Exemplo com Mais Parâmetros
    - Mais de um Parâmetro
    - Retorno em Funções
    - Função com Valores Padrão para Argumentos
    - Função com Números Arbitrários de Parâmetros
    - Funções com Argumentos Arbitrários
    - Função Recursiva
    - Funções Aninhadas
    - Calculadora com Funções Aninhadas
    - Funções Built-in
    - Funções Built-in de Strings
19. Interface Gráfica

## 1. Introdução <a name="introducao"></a>

Introdução ao Python, incluindo a execução de comandos básicos:

```python
print("Hello world!")
print("Olá mundo")
a = "Leandro "
b = "Barbosa"
print(a + b)

```

## 2. Comentários em Python <a name="comentarios"></a>

Como adicionar comentários no código:

```python
print("Olá!")
# Este é um comentário
'''
Comentário com mais de uma linha
'''

```

## 3. Variáveis <a name="variaveis"></a>

### Tipos de Variáveis

Trabalhando com diferentes tipos de variáveis:

```python
a = "Leandro"
b = 'Barbosa'
c = '''Vieira'''
print(a + b + c)

```

### Strings

Manipulação e formatação de strings:

```python
nome = "Rua Manoel Paiva \\nN°325\\nBairro Parque Piauí\\nTimon/MA"
print(nome)

```

### Números

Operações com números inteiros e reais:

```python
numero = 10
numero_real = 5.5
resultado = numero + numero_real
print(resultado)

```

## 4. Operadores Aritméticos <a name="operadores"></a>

Uso de operadores matemáticos:

```python
a = 3
b = 4
print(a == b)
print(a != b)
print(a + b)

```

## 5. Identação <a name="identacao"></a>

Importância da identação no Python:

```python
if a > b:
    print("A é maior que B")
else:
    print("A é menor que B")

```

## 6. Entrada de Comandos <a name="entrada"></a>

Capturando entradas do usuário:

```python
nome = input("Digite seu nome: ")
print(f"Nome: {nome}")

```

## 7. Exercícios <a name="exercicios"></a>

Exercícios práticos para reforçar o aprendizado:

```python
# 1) Que imprima números de 1 a 10.
for i in range(10):
    print(i + 1)

```

## 8. Casting <a name="casting"></a>

Mudança de tipos de variáveis:

```python
texto1 = "1.5"
numero1 = float(texto1)
print(numero1)

```

## 9. Manipulação de Strings <a name="strings"></a>

### Invertendo Strings

```python
texto = "ROMA"
print(texto[::-1])

```

### Testando a Existência de Caracteres

```python
texto1 = "Casa"
print("a" in texto1)

```

### Imutabilidade

```python
texto = "estudo python 3"
texto = texto.replace("3", "2")
print(texto)

```

### Métodos

```python
texto = "estudo python 3"
print(texto.capitalize())

```

## 10. Formatação de Strings <a name="formatacao"></a>

```python
print("A pontuação total de {} foi {} pontos".format("Fernando", "10"))

```

## 11. Comandos de Decisão <a name="decisao"></a>

Uso de if, else e elif:

```python
numero = int(input("Digite um número: "))
if numero < 10:
    print("Menor que 10")
elif numero < 100:
    print("Menor que 100")
else:
    print("Maior ou igual a 100")

```

## 12. Laços de Repetição <a name="lacos"></a>

### While

```python
num = 0
while num < 5:
    print(num)
    num += 1

```

### For

```python
for i in range(10):
    print(i)

```

## 13. Listas <a name="listas"></a>

Manipulação de listas e suas operações:

```python
lista = [1, 2, 3, 4]
lista.append(5)
print(lista)

```

## 14. Conjuntos (Sets) <a name="sets"></a>

Operações com conjuntos:

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
set_unido = set1.union(set2)
print(set_unido)

```

## 15. Tuplas <a name="tuplas"></a>

Uso de tuplas:

```python
tupla = (1, 2, 3)
print(tupla[0])

```

## 16. Dicionários <a name="dicionarios"></a>

Trabalhando com dicionários:

```python
idades = {'Ana': 16, 'Carol': 20}
print(idades['Ana'])

```

## 17. Lista Comprehensions <a name="comprehensions"></a>

Sintaxe e exemplos de lista comprehensions:

```python
lista = [x for x in range(0, 11)]
print(lista)

```

## 18. Funções

```markdown

Função em Python é definida com `def`.

### Exemplo de Definição de Função

```python
def qualquercoisa():
    num = 10
    print(f"uma função {num}")
qualquercoisa()

```

### Função que "não faz nada"

```python
def frankstains():
    pass
frankstains()

```

### Parâmetros em Função

```python
def print_var(numero):
    print(numero)
print_var(2)

```

### Exemplo de Soma

```python
def sum(a, b):
    return a + b
c = sum(5, 3)
print(c)

```

### Exemplo com Mais Parâmetros

```python
def sum(a, b, c, d):
    return a + b + c + d
c = sum(5, 3, 6, 9)
print(c)

```

### Mais de um Parâmetro

```python
def soma(num1, num2):
    print(num1 + num2)
soma(3, 2)
soma("Olá", "Mundo")
soma(3.0, 2.4)

```

### Retorno em Funções

```python
def subtrai(num1, num2):
    valor = num1 - num2
    return valor
subtracao = subtrai(10, 4)
print(subtracao)

```

### Função com Valores Padrão para Argumentos

```python
def salario_descontado_imposto(salario, imposto=27.5):
    return salario - (salario * imposto * 0.01)
print(salario_descontado_imposto(5000))

```

### Função com Números Arbitrários de Parâmetros

```python
def func(*args):
    print(type(args))
    print("Argumentos são: ", args)
func()
func(1, 2, 3)
func(12, "a", 'b', 3.14, [1, 2, 3, 4, 5], True)

```

### Funções com Argumentos Arbitrários

```python
def func(**args):
    print(type(args))
    print(args)
    print(args["Valor"])
func(Valor=10, operacao='soma', resultado=10)

```

### Função Recursiva

```python
def conta(numero):
    print(numero)
    if numero >= 10:
        return
    conta(numero + 1)
conta(5)

```

### Funções Aninhadas

```python
def pai():
    def filho():
        print("Eu sou filho")
        def neto():
            print("Eu sou neto")
        neto()
    filho()
    print("Agora sou Pai")
pai()

```

## Calculadora com Funções Aninhadas

```python
def calculadora(num1, num2, op):
    def soma(x, y):
        return x + y
    def subtrai(a, b):
        return a - b
    def mult(a, b):
        return a * b
    def divi(j, z):
        return a / b

    if op == '+':
        return soma(num1, num2)
    elif op == '-':
        return subtrai(num1, num2)
    elif op == '*':
        return mult(num1, num2)
    elif op == '/':
        return divi(num1, num2)
    else:
        print('Operação inválida!')
print(calculadora(100, 4, '+'))

```

### Funções Built-in

```python
print(abs(-10*4))
print(max(10, 20, 30, 40, 50))
print(min(10, 20, 30, 40, 50))
print(pow(2, 3))

import math
print(math.sqrt(25))
print(round(5.345))
print(round(5.345, 2))
print(math.ceil(5.345))
print(math.floor(5.345))
print(divmod(10, 4))

```

### Funções Built-in de Strings

```python
texto = "21212123333333"
print(texto.count("1"))
print(texto.startswith("21"))
print(texto.endswith("339"))
print(texto.replace("@", "a"))
print(texto.split(":"))
print("abcdE3".isalpha())
print("123".isdigit())
print("0".isdecimal())
print("abcsE3".isalnum())
print("   ".isspace())
print("isTo É esTRanhO".lower())
print("isTo É esTRanhO".upper())
print("isTo É esTRanhO".capitalize())
print("isTo É esTRanhO".swapcase())

numero = 70
print(f"O numero {numero} é lido pelo caractere {chr(numero)}")

for i in range(0, 127):
    print(f'{i} = {chr(i)}')

caractere = "a"
print(ord(caractere))

lista = [5, 10, 2, 1, 5, 10]
lista_nomes = ["Zelda", "Ana", "Teresa", "Beatriz", "Gilda"]
lista.sort()
lista_nomes.sort()
print(lista)
print(lista_nomes)

lista.sort(reverse=True)
lista_nomes.sort(reverse=True)
print(lista)
print(lista_nomes)

produtos = [['carro','R$ 100.000'], ['caceira','R$ 1000'], ['Moto','R$ 40000'], ['geladeira','R$ 20000'], ['armário','R$ 1500']]
for produto, valor in produtos:
    print(produto, "- ", valor)

import datetime
data_completa = datetime.datetime.now()
data = data_completa.date()
hora = data_completa.time()
print(data_completa)
print(hora)
print(data)
data2 = data.strftime("%d/%m/%Y")
print(data2)
data2 = data.strftime("%d-%m-%Y")
print(data2)
data2.format("%d-%m-%Y")
print(data2)
hora = datetime.time(10, 20, 30)
print(hora)

current_time = data.strftime("Data: %y/%m/%d \\nHora: %H:%M:%S")
print(current_time)

```

### 19. Interface Gráfica

```python
from tkinter import *

janela = Tk()
janela.title("Minha janela")
janela.mainloop()

```
## Conclusão

Este notebook é uma introdução prática aos conceitos fundamentais do Python. Continue praticando e explorando novos recursos da linguagem para aprimorar suas habilidades.
