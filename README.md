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


21º Faça um programa em Python que abra e reproduza o áudio de um arquivo MP3.

import pygame
pygame.init()
pygame.mixer.music.load("TO VOANDO ALTO.mp3")
pygame.mixer.music.play()
pygame.event.wait()
    

22º Crie um programa que leia o nome completo de uma pessoa e mostre:

– O nome com todas as letras maiúsculas e minúsculas.

– Quantas letras ao todo (sem considerar espaços).

– Quantas letras tem o primeiro nome.

resposta:

n = str(input('Digite seu nome completo:')).strip()
n_s_e = n.replace( ' ', '')
c = len(n_s_e)
p_n = n.split()[0]
c_p_n = len(p_n)
print(f' \n Nome com as letras em Maiúsculas -> {n.upper()}.')
print('-'*65)
print(f' Nome com as letras em Minúsculas -> {n.lower()}.')
print('-'*65)
print(f' A quantidade de letras SEM os espaços são de -> {c} números.')
print('-'*65)
print(f' A quantida de letras do 1º nome são de -> {c_p_n} números.')


23º Faça um programa que leia um número de 0 a 9999 e mostre na tela cada um dos dígitos separados.

resposta:

num = input("Digite um número de \"0\" a \"9999\": ")

digitos = [int(digito) for digito in str(num)]

while len(digitos) < 4:
    digitos.insert(0, 0)

digito1 = digitos[0]
digito2 = digitos[1]
digito3 = digitos[2]
digito4 = digitos[3]

print(f"Milhar: {digito1}\nCentena: {digito2}\nDezena: {digito3}\nUnidade: {digito4}")


24º Crie um programa que leia o nome de uma cidade diga se ela começa ou não com o nome “SANTO”.

resposta:

n = str(input('Digite o nome da cidade:')).strip().title()
n_s_e = n.split()

if n_s_e[0] == 'Santo':
    print('O nome dessa cidade começa com SANTO')

else:
    print('O nome dessa cidade não começa com  SANTO')


25º Crie um programa que leia o nome de uma pessoa e diga se ela tem “SILVA” no nome.

resposta:

n = str(input('Digite um nome \033[1;34mCOMPLETO\033[m: ')).strip().title().split()

if 'Silva' in n:
    print('Esse nome \033[1;32mtem SILVA\033[m')
else:
    print('Esse nome \033[1;31mnão\033[m tem \033[1;31mSILVA\033[')


26º Faça um programa que leia uma frase pelo teclado
 e mostre quantas vezes aparece a letra “A”, 
 em que posição ela aparece a primeira vez
 e em que posição ela aparece a última vez.

resposta:

n = str(input('Escreva uma frase:')).title().strip()

c_n = n.replace(' ','') 
c_a = n.count('A') + n.count('a')  # Contar ocorrências de 'a' e 'A' separadamente
p_a = n.find('a') + 1  # Adicionar 1 para contar a partir da primeira posição corretamente
u_a = c_n.rfind('a') + 1  # Adicionar 1 para contar a partir da última posição corretamente

print(f'A letra \'A\' apareceu {c_a} vezes.')
print(f'A letra \'A\' apareceu pela primeira vez na {p_a}º posição da frase.')
print(f'A letra \'A\' apareceu pela última vez na {u_a}º posição da frase.')


27º Faça um programa que leia o nome completo de uma pessoa, mostrando em seguida o primeiro e o último nome separadamente.

resposta:

n = str(input('Digite o nome:')).title().strip()

n_b = n.split()

print(n)
print(f'O 1º nome é {n_b[0]} e o último nome é {n_b[-1]}.')


28º Escreva um programa que faça o computador “pensar” em um número inteiro entre 0 e 5
e peça para o usuário tentar descobrir qual foi o número escolhido pelo computador.
O programa deverá escrever na tela se o usuário venceu ou perdeu.

resposta:

from random import choice
from time import sleep

lista = [0, 1, 2, 3, 4, 5]
num_sorteado = choice(lista)

print("-=-" * 20)
print("Vou pensar em um número entre 0 e 5. Tente adivinhar...")
print("-=-" * 20)

while True:
    jogador = int(input("Digite um número de 0 a 5: "))
    print("PROCESSANDO...")
    sleep(1)

    if jogador == num_sorteado:
        print("-=-" * 20)
        print("Parabéns! Você conseguiu me vencer!")
        print("-=-" * 20)
        break
    else:
        print("-=-" * 20)
        print("Você errou! O número sorteado foi: {}\nTente novamente.".format(num_sorteado))
        print("-=-" * 20)
        num_sorteado = choice(lista)  


29º Escreva um programa que leia a velocidade de um carro. Se ele ultrapassar 80Km/h, mostre uma mensagem dizendo que ele foi multado. A multa vai custar R$7,00 por cada Km acima do limite.

resposta:

v = float(input('Digite a velocidade do carro:'))
multa = v - 80
if v >= 80:
    print('Você foi \033[1;31mmultado\033[m')
    print(f'valor total da multa \033[1;32mR$ {multa * 7 }\033[m')


30º Crie um programa que leia um número inteiro e mostre na tela se ele é PAR ou ÍMPAR

resposta:

n = int(input('Digite um número:'))

if n  % 2 == 0:
    print(f'{n} é \033[1;32mPAR\033[m')
else:
    print('Muito bem! prossiga sua viagem')


 31º Desenvolva um programa que pergunte a distância de uma viagem em Km. 
 Calcule o preço da passagem, cobrando R$0,50 por Km para viagens de até 200Km e R$0,45 parta viagens mais longas.

 resposta:

d = float(input('Digite a distância da viagem em KM:'))

if d  <= 200:
    preço = d * 0.50
    print(f'A viagem com a quilometragem {d}KM será de {preço}')
elif d >= 201:
    preço = d * 0.45
    print(f'A viagem com a quilometragem {d}KM será de {preço}')

else:
    print('Valor Inválido!')


32º  Faça um programa que leia um ano qualquer e mostre se ele é bissexto.

resposta:

from datetime import date 

ano = int(input("Que ano quer analizar? Coloque 0 para analizar o ano atual :"))
if ano == 0:
    a_a = date.today().year
    print(a_a)
elif  ano % 4 == 0 and ano % 100 != 0  or ano % 400 == 0:
    print('Esse ano é bissexto')

else:
    print('Esse ano não é bissexto')


33º  Faça um programa que leia três números e mostre qual é o maior e qual é o menor.

resposta:

n1 = int(input('Digite o 1º número:'))
n2 = int(input('Digite o 2º número:'))
n3 = int(input('Digite o 3º número:'))

if n1 > n2 and n1 > n3:
    print(f'O número {n1} é o MAIOR ')
elif n2 > n1 and n2 > n3:
    print(f'O número {n2} é o MAIOR número')
else:
    print(f'O número {n3} é o MAIOR número')


34º Escreva um programa que pergunte o salário de um funcionário e calcule o valor do seu aumento. Para salários superiores a R$1250,00, calcule um aumento de 10%. Para os inferiores ou iguais, o aumento é de 15%

resposta:

s = float(input('Digite seu SALÁRIO:'))

if s > 1250:
    s_a = (1250 * 10) / 100
    print(f'O total salário no valor de {s} com o novo aumento é de {s_a}')
elif s <= 1250:
    s_a = (1250 * 15) / 100
    print(f'O total do salário no valor de {s} com o novo aumento é de R$ {s_a}')


35º Desenvolva um programa que leia o comprimento de três retas e diga ao usuário se elas podem ou não formar um triângulo.

resposta:

r1 = float(input("Digite o comprimento da 1º linha: "))
r2 = float(input("Digite o comprimento da 2º linha: "))
r3 = float(input("Digite o comprimento da 3º linha: "))

if r1 + r2 > r3 and r1 + r3 > r2 and r2 + r3 > r1:
    print("Triângulo deu certo, mano.")
else:
    print("Infelizmente não formou o triângulo.")


36º Escreva um programa para aprovar um empréstimo bancário para a compra de uma casa. Pergunte o valor da casa, o salário do comprador e em quantos anos ele vai pagar. A prestação mensal não pode exceder 30% do salário ou então o empréstimo será negado.

resposta:

c = float(input('Qual o valor da casa?'))
s = float(input('Qual o valor do seu salário?'))
a = int(input('Quantos anos você deseja pagar ?:'))
 
parcela = c /  (a * 12)
porcentagem = (s * 30) / 100

if parcela > porcentagem:
    print (f'Empréstimo não concedido \n Valor da parcela é de {parcela:.5f}')

else:
    print (f'Empréstimo concedido. Valor da parcela é de {parcela:.5f}')

print(f'Valor da parcela é de {parcela:.5f}')


37º Escreva um programa em Python que leia um número inteiro qualquer e peça para o usuário escolher qual será a base de conversão: 1 para binário, 2 para octal e 3 para hexadecimal.

resposta:

num = int(input("Digite um número INTEIRO:"))
base = int(input("Digite qual a base de conversão você deseja. \n 1 - para BINÁRIO. \n 2 - para OCTAL. \n 3 - para hexadecimal \n reponda:"))


binário = bin(num)[2:]
octal  = oct(num)[2:]
hexadecimal = hex(num)[2:]


if base == 1:
    print("O valor BINÁRIO deste numero é {}".format(binário))

elif base == 2:
    print("O valor OCTAL deste número é {}".format(octal))

elif base == 3:
    print("O valor HEXADECIMAL deste número é {}".format(hexadecimal))


38º Escreva um programa que leia dois números inteiros e compare-os. mostrando na tela uma mensagem:

– O primeiro valor é maior

– O segundo valor é maior

– Não existe valor maior, os dois são iguais

resposta:

num1 = int(input("Digite o PRIMEIRO NÚMERO:"))
num2 = int(input("Dgite o SEGUNDO NÚMERO:"))

if num1 >  num2:
    print("O primeiro valor: \033[1;4;34m{}\033[m é maior do que o segundo valor: \033[1;4;31m{}\033[m".format(num1,num2))
elif num1 < num2:
    print("O primeiro número:  \033[1;4;34m{}\033[m é menor do que o segundo valor:  \033[1;4;31m{}\033[m".format(num1,num2))
else:
    print("nâo existe valor maior, os dois são \033[1;4;34mIGUAIS\033[m.")


39º Faça um programa que leia o ano de nascimento de um jovem e informe, de acordo com a sua idade, se ele ainda vai se alistar ao serviço militar, se é a hora exata de se alistar ou se já passou do tempo do alistamento. Seu programa também deverá mostrar o tempo que falta ou que passou do prazo.

resposta:

from datetime import datetime
nascimento = int(input("Qual o ANO que você nasceu ?"))
ano_atual = datetime.now().year
idade = ano_atual - nascimento



if  idade ==  18 : 
   print("Você deve se alistar.")

elif idade >= 18 and idade <= 45:
   print("você ainda pode se alistar.") 
elif idade < 18:
   print("Você não pode se alistar ainda.")
else:
   print("Seu tempo para se alistar expirou")


40º Crie um programa que leia duas notas de um aluno e calcule sua média, mostrando uma mensagem no final, de acordo com a média atingida:

– Média abaixo de 5.0: REPROVADO

– Média entre 5.0 e 6.9: RECUPERAÇÃO

– Média 7.0 ou superior: APROVADO

resposta:

n1 = float(input("Digite a primeira nota:"))
n2 = float(input("Digite a segunda nota:"))
notas = (n1,n2)
media = sum(notas) / len(notas)

if media <= 5:
    print("\033[1;4;31mReprovado\033[m")
elif media >= 5 and media <= 6.9:
    print("\033[1;4;34mRecuperação\033[m")
else:
    print("\033[1;4;32mAprovado\033[m")


41º A Confederação Nacional de Natação precisa de um programa que leia o ano de nascimento de um atleta e mostre sua categoria, de acordo com a idade:

– Até 9 anos: MIRIM

– Até 14 anos: INFANTIL

– Até 19 anos: JÚNIOR

– Até 25 anos: SÊNIOR

– Acima de 25 anos: MASTER

resposta:

i = int(input('Digite a idade do Atleta:'))

if i <= 9:
    print('A categoria é MIRIM')
elif i > 9 and i <= 14:
    print('A categoria é INFANTIL')
elif i > 14 and i <= 19:
    print('A categoria  é JUNIOR')
elif i > 19 and i <= 25:
    print('A categoria  é SENIOR')
else:
    print('A categoria é MASTER')`


42º Refaça o DESAFIO 35 dos triângulos, acrescentando o recurso de mostrar que tipo de triângulo será formado:

– EQUILÁTERO: todos os lados iguais

– ISÓSCELES: dois lados iguais, um diferente

– ESCALENO: todos os lados diferentes

reposta:

r1 = float(input("Digite o comprimento da 1º linha: "))
r2 = float(input("Digite o comprimento da 2º linha: "))
r3 = float(input("Digite o comprimento da 3º linha: "))

if r1 + r2 > r3 and r1 + r3 > r2 and r2 + r3 > r1:
    if r1 == r2 == r3:
        print('Esse triângulo é um EQUILÁTERO')
    elif r1 == r2 or r1 == r3 or r2 == r3:
        print('Esse triângulo é um ISÓSCELES')
    else:
        print('Esse triângulo é um ESCALENO')
else:
    print('Infelizmente não formou um triângulo.')


43º Desenvolva uma lógica que leia o peso e a altura de uma pessoa, calcule seu Índice de Massa Corporal (IMC) e mostre seu status, de acordo com a tabela abaixo:

– IMC abaixo de 18,5: Abaixo do Peso

– Entre 18,5 e 25: Peso Ideal

– 25 até 30: Sobrepeso

– 30 até 40: Obesidade

– Acima de 40: Obesidade Mórbida

resposta:

p = float(input('Digite seu PESO:'))
a = float(input('Digite sua ALTURA:'))

imc = p / (a**2)

if  imc < 18.5:
    print('ABAIXO do peso')
elif imc >= 18.5 and imc  < 25:
    print('peso IDEAL')
elif imc >=  25 and imc < 30:
    print('Sobrepeso')
elif  imc >= 30 and imc <= 40:
    print('OBSOBIDADE MORBIDA')













































 




