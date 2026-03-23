# Exercício 01

## Gerar Dicionário Quadrado
Criar uma função Python que toma um número inteiro (n) como entrada e gera um dicionário contendo pares ( (i, i^2) ) para todos os números inteiros (i) de 1 a (n) (inclusive). A função deverá então retornar este dicionário.

### Código Simples:

    i = int(input("Digite um número inteiro: "))
    n = {i: i * i}
    
    print(f"O valor será {n}")

Saída:

  Digite um número inteiro: 3
  
  O valor será {3: 9}

### Com o Dicionário:

    def dicionario_quadrado(n):
        resultado = dict()
        for i in range(1, n + 1):
            resultado[i] = i * i
        return resultado
        
    print(dicionario_quadrado(5))

Saída:

{1: 1, 2: 4, 3: 9, 4: 16, 5: 25}

### Comentários:

    def dicionario_quadrado(n):     # Cria uma função "dicionario_quadrado" que recebe o valor de "n".
        resultado = dict()           # Cria um dicionário vazio com o nome de "resultado".
        for i in range(1, n + 1):     # Inicia um laço de repetição "for" para repetir cada numero "i" de 1 até n.
            resultado[i] = i * i       # Cria uma chave "i" no dicionário, onde o valor será "i * i".
        return resultado                 # Retorna o dicionário preenchido com o "resultado".
        
    print(dicionario_quadrado(5))         # Mostra na tela o que foi calculado até o 5.
