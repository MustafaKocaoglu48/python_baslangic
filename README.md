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











