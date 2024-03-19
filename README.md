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


4º Faça um programa que leia algo pelo teclado e mostre 
   na tela o seu tipo primitivo
   e todas as informações possíveis sobre ele.

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



 




