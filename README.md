# (20) Considerando a matriz abaixo, crie um laço for para calcular a média de uso de CPU por linha e imprima os resultados com 2 casas decimais.


uso_cpu = [
[20, 25, 40, 50, 45, 60, 55, 35, 70, 65],
[30, 35, 50, 60, 40, 55, 60, 45, 50, 55],
[15, 20, 30, 25, 35, 40, 45, 50, 55, 60],
[10, 15, 25, 35, 45, 50, 55, 60, 65, 70],
]
for i in range(len(uso_cpu)):
  soma = 0
  for j in range(len(uso_cpu[i])):
    soma += uso_cpu[i][j]
  media =soma/len(uso_cpu[i])
  print(f'A média de uso de CPU na linha{i+1} é {media: .2f}')

  uso_cpu = [
    [20, 25, 40, 50, 45, 60, 55, 35, 70, 65],
    [30, 35, 50, 60, 40, 55, 60, 45, 50, 55],
    [15, 20, 30, 25, 35, 40, 45, 50, 55, 60],
    [10, 15, 25, 35, 45, 50, 55, 60, 65, 70],
]

def alerta_uso(lista):
    uso = 85
    for i in range(len(lista)): 
        for j in range(len(lista[i])):  
            if lista[i][j] > uso:  
                return True
    return False  


resultado = alerta_uso(uso_cpu)
print(resultado)

# 20) Crie uma função chamada dados_crescente que recebe como parâmetro uma lista com os valores de uso de CPU de uma região. A função deve retornar a lista organizada em ordem crescente, do menor uso de CPU para o maior. Teste a função para todas as regiões da matriz

uso_cpu = [
    [20, 25, 40, 50, 45, 60, 55, 35, 70, 65],
    [30, 35, 50, 60, 40, 55, 60, 45, 50, 55],
    [15, 20, 30, 25, 35, 40, 45, 50, 55, 60],
    [10, 15, 25, 35, 45, 50, 55, 60, 65, 70],
]

def dados_crescente(lista):
    for i in range(len(lista)):
        lista[i].sort() 

dados_crescente(uso_cpu)

print(uso_cpu)

# (20) Dentre as questões anteriores escolha uma delas para fazer uma leve explicação do seu funcionamento.
uso_cpu = [
    [20, 25, 40, 50, 45, 60, 55, 35, 70, 65],
    [30, 35, 50, 60, 40, 55, 60, 45, 50, 55],
    [15, 20, 30, 25, 35, 40, 45, 50, 55, 60],
    [10, 15, 25, 35, 45, 50, 55, 60, 65, 70],
]

def dados_crescente(lista):
    for i in range(len(lista)):
        lista[i].sort() 

dados_crescente(uso_cpu)

print(uso_cpu)

# Temos uma algumas listas separadas entre linhas e colunas, fiz um for para fazer uma vareadura no indice desta lista e apos isso fiz um metodo sort que organiza a lista do menor para o maior. Apos isso dei um print para vizualizar essa lista organzida.
