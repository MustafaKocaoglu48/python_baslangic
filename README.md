# python_baslangic
---
### ekrana yazma
````python
print("merhaba")
````
---
### Değişken tanımlama
````python
musteriAdi="Ali"
musteriSoyadi="Yilmaz"
print(musteriAdi+" "+musteriSoyadi)
musteriDogumYili=1987
musteriYasi=2022-musteriDogumYili
print(musteriYasi)
````
### Tip Dönüşümü
````python

x=5
y=2.5
name="Cınar"
tip=True

print(type(x))
print(type(y))
print(type(name))
print(type(tip))

x=float(x)
print(x)
print(type(x))

y=int(y)
print(y)
print(type(y))

topla=str(x)+str(y)
print(topla)
print(type(topla))


tip2=str(tip)
print(tip2)
print(type(tip2))

tip=int(tip)
print(tip)
print(type(tip))

````
### Dairenin alanı
````python
import math

Yaricap=input("Yaricap:"  )

Alan=int(Yaricap)*int(Yaricap)*math.pi
print(Alan)
Cevre=2*int(Yaricap)*math.pi
print(Cevre)
````
### İsim yazdırma
````python
Ad="Mustafa"
Soyad="Kocaooğlu"
Yas=20
print("AD:"+Ad+" "+Soyad+" \n YAŞ:"+str(Yas))
````
### String dizileri
````python
Ad="Mustafa"
Soyad="Kocaooğlu"
Yas=20
Tanıtma="AD:"+Ad+" "+Soyad+" \nYAŞ:"+str(Yas)

print(Tanıtma)
print(Tanıtma[1])
print(Tanıtma[5])
print(Tanıtma[len(Tanıtma)-1])
print(Tanıtma[2:8])
print(Tanıtma[2:])#Dizinin sonuna kadar gider
print(Tanıtma[:8])#En bastan baslar 8. karaktere kadar gider
print(Tanıtma[2:17:3])#3 er 3 er karakterleri aliyor
````
### String Formatlama
````python
Ad="Mustafa"
Soyad="Kocaooğlu"
Yas=20
Tanıtma="AD:"+Ad+" "+Soyad+" \nYAŞ:"+str(Yas)

print(Tanıtma)
print(Tanıtma[1])
print(Tanıtma[5])
print(Tanıtma[len(Tanıtma)-1])
print(Tanıtma[2:8])
print(Tanıtma[2:])#Dizinin sonuna kadar gider
print(Tanıtma[:8])#En bastan baslar 8. karaktere kadar gider
print(Tanıtma[2:17:3])#3 er 3 er karakterleri aliyor
````

### String metodları
````python
message="Hi There.My name is Mustafa KOCAOĞLU"

message=message.upper()# Tüm karakterleri büüyük yazar
message=message.lower() # Tüm karakyerleri küçük yazar
message=message.title()  #  Tüm karakterlerin baş harfini büyük yazar
message=message.capitalize()#  Sadece ilk harf büyük yazılır
message=message.strip()  #Baştaki boşluğu siler
message=message.split()   # Diziye atar
message=message.split('.')#  Konulan karaktere göre ayırır
message='---'.join(message)  # Her harfi  konulan karakter arasına alır
index=message.index('Mustafa')#   Parantez arasına alınan karakterin varsa kaçıncı indexte olduğunu söyler
message=message.startswith('H')# Karakter atanmıs değişken parantez içindeki harf ile mi basliyor
message=message.endswith("U")  #Karakter atanmıs değişken parantez içindeki harf ile mi bitiyor
message=message.replace('Mustafa','Ahmet')# Bulduğu tüm mustafa karaktetrleri yerine ahmet yazar
message=message.center(100,'*') #Mesajı 100 karakterli bir boşluğa atar ve bastan sona yıldız koyar ortaya da değişkeni atar
print(message)
````
### Python Listeleyici
````python
my_list=[1,2,3]
my_List=[1,'iki',True,4.7]

print(my_List)

list1=['one','two','three']
list2=['four','five','six']

numbers=list1+list2
print(numbers)

message="Hi there.My name is Mustafa KOCAOĞLU"
print(message[0])
message="Hi there.My name is Mustafa KOCAOĞLU".split()
print(message[0])

userA=['SADIK',30]
userB=['MUSTAFA',20]
print(userA)
print(userB)
users=[userB+userA]
print(users)
print(users[0][1])
````
### Liste Metodları
````python
numbers=[1,2,35,56,34,27,65,35,98,43,12]
letters=['a','v','e','s','d','s','g','m']

#val=min(letters)    Alfabeti sıraya göre a dan z ye doğru a harfine yakın olanı bulur
#val1=min(numbers)   sayısal olarak en küçüğünü bulur

#val2=max(letters) z ye daha yakın olanı bulur
#val3=max(numbers)    en büyük sayıyı bulur

#print(val)
#print(val1)
#print(val2)
#print(val3)
#numbers[4]=40
#print(numbers)

#
# numbers.append(13)   Listenin sonuna girile sayıyı ekler
#numbers.insert(2,34) belirlenen indise 34 sayısını ekler
#numbers.insert(-1,26)  sondan bir onceki sayyıya ekleme yapar.
#numbers.pop() en sondaki sayıyı siler,
#numbers.pop(2) parantez içindeki indesi siler
#numbers.remove(35) silmek istediğimiz sayıyı yazarız birden fazla varsa sadece ilkini siler

#umbers.sort() sayıları küçükten büyüğe doğru sıralar
#letters.sort() alfabetik sıralama yapar

#print(numbers.count(35) ) parantez içindeki sayıdan kaç tane oldulğunu söyler

#print(numbers.clear()) komple listeyi siler
````
### Karşılaştırma öperatörleri
````python
#Girilen 2 sayıdan hangisi daha büyüktür
'''
ilk_sayi=int(input("Bir sayı giriniz:"))
ikinci_sayı=int(input("2. sayıyı giriniz:"))
sonuc=(ilk_sayi<ikinci_sayı)
print(sonuc) #Dönen değer true ise 2.sayı daha büyüktür '''

#Kullanıcıdan vize ve final notu alınız kullanıcının geçme kalma 
# duurumuna göre ekrana kaldı geçti yazdırınız
'''
vize_notu=int(input("Vize notunu giriniz:"))*0.4
final_notu=int(input("Final notunu giriniz:"))*0.6
genel_not=vize_notu+final_notu
if genel_not<50:{        

print("Kaldı")} 
else:

 print("Geçti") '''

#Girilen sayının tek mi çift mi olduğunu bulma
'''
girilen_sayi=input("Bir sayı giriniz:")
if (int(girilen_sayi)%2==0):
            print("Sayı çift sayıdır.")
else:
 print("Girilen Sayı Tek")'''

#Parola ve e mail doğruluğunu kabul etme
'''
Girilen_email=input("Bir mail adresi giriniz:")
Girilen_Parola=input("E mail adresinin parolasını giriniz:")

email_adresi='mustafakocaoglu2018@gmail.com'
parola='123456'



result=(email_adresi==Girilen_email)
result2=(parola==Girilen_Parola)

print(f'Girilen email doğru mu? {result} Girilen parola doğru mu?{result2}')'''
````
### Python if-else yapısı
````python
'''
girilen_ilk_sayi=int(input("İlk sayıyı giriniz:"))
girilen_ikinci_sayı=int(input("İkinci sayıyı giriniz:"))

if girilen_ilk_sayi>girilen_ikinci_sayı:
   print("İlk sayı ikinci sayıdan büyüktür.")
elif girilen_ilk_sayi<girilen_ikinci_sayı:
  print("İkinci sayı ilk sayıdan büyüktür.")
else:
    print("İki sayı birbirne eşittir.") '''
'''
girilecek_sayi=int(input("Bir sayı giriniz:"))

if girilecek_sayi<0:
    print("Sayı negatiftir.")
elif girilecek_sayi>0:
 print("Sayı pozitiftir.")
else:
 print("Sayı nötrdür.")'''
````
### if-else örnekler
````python

'''
girilen_ilk_sayi=int(input("İlk sayıyı giriniz:"))
girilen_ikinci_sayı=int(input("İkinci sayıyı giriniz:"))

if girilen_ilk_sayi>girilen_ikinci_sayı:
   print("İlk sayı ikinci sayıdan büyüktür.")
elif girilen_ilk_sayi<girilen_ikinci_sayı:
  print("İkinci sayı ilk sayıdan büyüktür.")
else:
    print("İki sayı birbirne eşittir.") '''
'''
girilecek_sayi=int(input("Bir sayı giriniz:"))

if girilecek_sayi<0:
    print("Sayı negatiftir.")
elif girilecek_sayi>0:
 print("Sayı pozitiftir.")
else:
 print("Sayı nötrdür.")'''
````
### For örnekleri
````python
sayilar=[1,3,5,6,4,23,21,27,72]

# 3 e bölünen sayıları ekrana yazdıran programı yazınız.
'''
for a in sayilar:
    if(a%3==0):
        print(a)
'''
#sayilar listesindeki sayıların tplamı nedir?
'''
toplam=0
for a in sayilar:
   toplam=toplam+a
print(toplam)   '''

#sayialr listesindeki tek sayıarın karesini alan programı yazınız.
'''
for a in sayilar:
   if(a%2==1):
      print(a)
      '''
#5 ve daha az harften oluşan şehirleri ekrana yazdıran programı yazınız.

sehirler=['Ankara','Bursa','Rize','Muğla']
 
for a in sehirler:
    if(len(a)<=5):
      print(a)
````
### while döngüsü
````python
x=0
while True:         #Sonsuz döngü
    print(x)   

'''

'''
# 1den 100 e kadar olan sayıları yazar
x=0
while x<100:
    print(x)
    x+=1
  '''

# 1den 100 e kadar olan sayıları çift ve tek diye yazdırmak
'''
x=0
while x<100:
    if(x%2==0):
        print(f'{x} sayısı çifttir')
        x+=1
    else:
        print(f'{x} sayısı tektir')    
        x+=1
'''
````
### while örnekleri
````python
'''
sayilar=[1,3,5,43,23,24,54,65]

#Sayılar listesini ekrana yazdırın
i=0
while i<len(sayilar):
    print(sayilar[i])
    i+=1
'''
#Başlangıç ve bitiş değerlerini kullanıcıdan alıp aradaki tek sayıları ekran yazdıran programı yazınız.
'''
ilk_deger=int(input("ilk değeri giriniz:"))
ikinci_deger=int(input("ikinci değeri giriniz:"))

x=ilk_deger
while x<=ikinci_deger:
    if x%2==1:
        print(x)
        x+=1 
    else:
        x+=1
'''

#1 ile 100 arasındaki sayıları azalan şekilde yazan programı yazınız.
'''
deger=100
while deger>0:
    print(deger)
    deger-=1
'''

#Kullanıcıdan 5 adet sayı alıp sıralayan ve ekrana yazdıran programı yazınız.
'''
numbers=[]
i=0
while i<5:
    sayi=int(input('Bir sayı giriniz:'))
    numbers.append(sayi)
    i+=1

numbers.sort()  #Sıralamayı yapıyor
print(numbers)
'''
````
### Sayı bulma oyunu
````python
import random

sayi=random.randint(1,100)
hak=5
sayac=0

while hak>0:
    hak-=1
    sayac+=1
    tahmin=int(input('Tahmininizi giriniz:'))
  
    if sayi==tahmin:
        puan=100-(sayac-1)*20
        print(f'Tebrikler {sayac} adımda buldunuz.Toplam puanınız:{puan}')
        break
    elif sayi>tahmin:
        print('yukarı')

    else:
        print('aşağı')         
    if hak==0:
       print(f'Hakkınız bitti tuutulan sayı{sayi}')
````
### Metod örnekleri
````python
#Gönderilen bir kelimeyi ekranda istenildiği kadar yazan programı yazınız.
'''
def yazdir(adet,kelime):
    print(adet*kelime)

yazdir(12,'Merhaba\n')    
'''
#Kendisine gönderilen sınırsız sayıdaki parametreyi listeye atayan  metodu yazınız.
'''
def listeyecevir(*params):
    liste=[]
    for param in params:
        liste.append(param)
      
    return liste

result=listeyecevir('Merhaba',23,12,54,32)
print(result)
'''

#Gönderilen 2 sayı arasındaki asal sayıların tümünü yazan metod.
'''
def asalsayi_bul(sayi1,sayi2):
    for sayi in range(sayi1,sayi2+1):
        if sayi > 1:
          for i in range(2,sayi):
              if(sayi % i ==0):
                  break
          else:
                print(sayi)

sayi1=int(input('Birinci sayıyı giriniz:'))
sayi2=int(input('İkinci sayıyı giriniz:'))

asalsayi_bul(sayi1,sayi2)
'''
#Kendisine gelen sayının tam bölenlerini yazdıran metodu yazınız.
'''
def tam_bolenler(sayi):
    tam_bolenler=[]

    for i in range(2,sayi):
        if(sayi % i ==0):
            tam_bolenler.append(i)
    
    return tam_bolenler

print(tam_bolenler(20))    
'''

````
### Lambda fonksiyonu
````python
'''
def square(num):
    return num**2

result=square(2)
print(result)
'''
'''
def square(num): return num**2

numbers=[1,3,4,5,6,13]

result=list(map(square,numbers))
print(result)
'''
'''
numbers=[1,2,3,4,20,12]
def square(num):
    return num**2

for i in map(square,numbers):
    print(i)
'''
'''
numbers=[2,3,4,6,3,7]
result=list(map(lambda num:num**2,numbers))

print(result)
'''
'''
square=lambda num:num**2
numbers=[2,3,7,3,6,8,5]
result=list(map(square,numbers))
print(result)
'''
````
### Global ve Local değişkenler
````python
x='global x'

def function():
     x='local x'
     print(x)

function()
print(x)    
#############################################################

name='cinar'  #Global tanımlama  yaptık

def change_name(new_name):
    #Local değişken olarak tanımladık
    name=new_name   
    print(name)

change_name('Mustafa')
print(name)

###############################################################

name='global'
# Burada hello metoduna göre çınar ismi global değişkendir.
def greeting():
    name='cinar'
    def hello():
        print('hello '+name)
    hello()

greeting()

#################################################################

x=50

def test(x):
   
    print(f'x:{x}')
    x=100
    print(f'x in yeni hali{x}')
    
test(x)
print(x)

# x bilgisini global tanımlamak istiyorsak test metodunu sileriz ve x i metod içine alıp 
#global tanımlarız.

x=50

def test():
   global x
   print(f'x:{x}')
   x=100
   print(f'x in yeni hali{x}')
    
test()
print(x)


````

