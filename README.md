# Exercicios Python
Aqui, estarão os exercícios que  resolvi do 'Curso-em-video', do curso de python.
Para saber mais sobre esse curso [clique aqui](https://www.cursoemvideo.com/curso/python-3-mundo-1/)


1º Crie um programa que escreva 'Olá, Mundo' na tela.
print('Olá, Mundo!')

Resposta:

print('Olá, Mundo!')


2º Faça um programa que 'leia' o nome de uma pessoa e mostre uma mensagem de 'boas-vindas'.

reposta:

nome = str(input('Digite seu nome: ')).capitalize().strip()
print(f'Bem vindo, {nome}!!!')


3º Crie um programa que leia dois números e mostre a soma entre eles

resposta:

n1 = float(input(("Digite o primeiro número:")))
n2 = float(input(("Digite o segundo número:")))
soma = n1 + n2

print(f'A soma dos  valores {n1} + {n2} = {soma}')


4º Faça um programa que leia algo pelo teclado e mostre na tela o seu tipo primitivo e todas as informações possíveis sobre ele.

resposta:

t = input('Digite alguma coisa: ')

print(f'O tipo primitivo desse valor é {type(t)}')
print(f'É um número ? {t.isnumeric()}')
print(f'É Alfabetico {t.isalpha()}')
print(f'É Alfanumérico? {t.isalnum()}')
print(f'Está em Maiúsculo? {t.isupper()}')
print(f'Está em minuscula? {t.islower()}')
print(f'Está capitalizada? {t.istitle()}')


5º Faça um programa que leia um número Inteiro e mostre na tela o seu sucessor e seu antecessor.

resposta:

n = int(input('Digite um valor:'))

print(f'O antecessor do valor {n}, é {n - 1} e seu sucessor é {n + 1}')


6º Crie um algoritmo que leia um número e mostre o seu dobro, triplo e raiz quadrada

resposta:

n = float(input(('Digite um numero:')))
d = dobro(n)
t = triplo(n)
r = n ** (1/2)

print(f"Os valores correspondentes são: \n{d}; \n{t}; \n{r}")


7º Desenvolva um programa que leia as duas notas de um aluno, calcule e mostre a sua média.
 
resposta:

nota1 = float(input('Digite a 1º nota:'))
nota2 = float(input('Digite a 2º nota:'))
notas = nota1, nota2
media = sum(notas)/len(notas) 

print(f'A MÉDIA das notas  é {media} ')


8º  Escreva um programa que leia um valor em metros e o exiba convertido em centímetros e milímetros.

resposta:

v =  float(input("Digite um valor em metros:"))
c = v * 100
m = v * 1000

print(f"Os valores convertidos são {c}cm, e {m}mm. ")


9º Faça um programa que leia um número Inteiro qualquer e mostre na tela a sua tabuada. (1º forma ensinada)

resposta:

n = float(input('Digite um valor: '))

print(f"{n} x 1 = {n*1} \n{n} x 2 = {n*2} \n{n} x 3 = {n*3} \n{n} x 4 = {n*4} \n{n} x 5 = {n*5} \n{n} x 6 = {n*6} \n{n} x 7 = {n*7} \n{n} x 8 = {n*8} \n{n} x 9 = {n*9} \n{n} x 10 = {n*10} ")
print("_"*15)


10º Crie um programa que leia quanto dinheiro uma pessoa tem na carteira e mostre quantos dólares ela pode comprar.

resposta:

nome = str(input('Qual é seu nome? ')).strip().capitalize()
reais = float(input('Quantos R$ você tem na carteira, {nome} ?'))
cambio_dolar = 5,03
compra_dolar = reais / cambio_dolar

print(f"{nome}, você poderia comprar {compra} dolares")


11º  Faça um programa que leia a largura e a altura de uma parede em metros, calcule a sua área e a quantidade de tinta necessária para pintá-la, sabendo que cada litro de tinta pinta uma área de 2 metros quadrados.

resposta:

altura = float(input('Digite a ALTURA em METROS: '))
largura = float(input('Digite a LARGURA em METROS:'))

a = altura * largura
tt = a / 2

print(f'A área da parede é {a} e a quantidade de tinda a ser usada é {tt}.')


12º Faça um algoritmo que leia o preço de um produto e mostre seu novo preço, com 5% de desconto

resposta:

p = float(input('Digite o PREÇO do produto:'))
pc = (p * 5)/100
n_p = p - pc

print(f'O preço do produto com o seu desconto é de R$ {n_p}')


13º Faça um algoritmo que leia o salário de um funcionário e mostre seu novo salário, com 15% de aumento.

resposta:

s = float(input('Digite o SALÁRIO do funcionário:'))
pc = (s * 15) / 100 
n_s = s + pc

print(f'O NOVO SALÁRIO do funcionário com 15% de acrescimo é de R$ {n_s}')


14º Escreva um programa que converta uma temperatura digitando em graus Celsius e converta para graus Fahrenheit.

resposta:

c = float(input('Digite a temperatura em GRAUS CELSIUS: '))
c_f = c * 1.8 + 32

print(f' A temperatura de CELSIUS para FAHRENHEIT é {c_f}Fº')


15º Escreva um programa que pergunte a quantidade de Km percorridos por um carro alugado e a quantidade de dias pelos quais ele foi alugado. Calcule o preço a pagar, sabendo que o carro custa R$60 por dia e R$0,15 por Km rodado.

resposta:

km = float(input('Digite a quantidade de KM PERCORRIDA pelo carro:'))
d = int(input('Digite a quantidade de DIAS que o carro foi alugado:'))

v_d = 60 * d
v_km = km * 0.15
p_f = v_d + v_km

print(f'O valor TOTAL a ser pago é de R$ {p_f}')


16º Crie um programa que leia um número Real qualquer pelo teclado e mostre na tela a sua porção Inteira.

resposta:

from math import trunc

n = float(input('Digite  um número real: '))
print(f'A porção INTEIRA do número digitado é {trunc(n)}')


17º Faça um programa que leia o comprimento do cateto oposto e do cateto adjacente de um triângulo retângulo. Calcule e mostre o comprimento da hipotenusa.
 
resposta:

from math import hypot
oposto = float(input('Digite o comprimento do cateto OPOSTO:'))
adjacente = float(input('Digite o comprimento do cateto ADJACENTE:'))

hipo = hypot(oposto, adjacente)

print(f'O valor da HIPOTENUSA é {hipo}')


18º Faça um programa que leia um ângulo qualquer e mostre na tela o valor do seno, cosseno e tangente desse ângulo.
 
resposta: 

from math import sin, cos, tan, radians

a = float(input('Digite o valor de um ÂNGULO: '))

a_radianos = radians(a)

seno = sin(a_radianos)
cosseno = cos(a_radianos)
tangente = tan(a_radianos)

print(f'O valor do SENO é {seno}\nO do COSSENO é {cosseno}\nE da TANGENTE é {tangente}')

 
 
19º Um professor quer sortear um dos seus quatro alunos para apagar o quadro. Faça um programa que ajude ele, lendo o nome dos alunos e escrevendo na tela o nome do escolhido.

resposta:

import random
alunos = []
aluno = 1

for i in range(4):
    nome = str(input(f'Digite o nome do {aluno}º aluno(a):')).capitalize().strip()
    alunos.append(nome)
    aluno += 1

random.shuffle(alunos)
aluno_escolhido = random.choice(alunos)

print(f'\nO aluno(a) escolhido(a) foi: {aluno_escolhido}')


20º O mesmo professor do desafio 19 quer sortear a ordem de apresentação de trabalhos dos alunos. Faça um programa que leia o nome dos quatro alunos e mostre a ordem sorteada.

resposta:

import random
alunos = []
aluno = 1

for i in range(4):
    nome = str(input(f'Digite o nome do {aluno}º aluno(a):')).capitalize().strip()
    alunos.append(nome)
    aluno += 1

random.shuffle(alunos)
lista_embaralhada = random.sample(alunos, len(alunos))

print(f'\nO aluno(a) escolhido(a) foi: {lista_embaralhada}')
    




 




