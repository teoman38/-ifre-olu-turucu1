# -ifre-olu-turucu1
import random
import string

rakamlar = string.digits
semboller = string.punctuation
kucuk_harfler = string.ascii_lowercase
buyuk_harfler = string.ascii_uppercase
tum_karakterler = [rakamlar, semboller, kucuk_harfler, buyuk_harfler]

sifre =("")

'''

for i in range(2):
    sifre += tum_karakterler[0][random.randint(0, 9)]
    
for i in range(2):
    sifre += tum_karakterler[1][random.randint(0, 9)]

for i in range(2):
    sifre += tum_karakterler[2][random.randint(0, 9)]

for i in range(2):
    sifre += tum_karakterler[3][random.randint(0, 9)]

'''
for j in range(4):
    for i in range(2):
        sifre += tum_karakterler[j][random.randint(0, 9)]

sifre = list(sifre)                     #şifre string oldu
random.shuffle(sifre)


yeni_sifre = ""
for i in sifre:
    yeni_sifre += i
print(yeni_sifre)    
