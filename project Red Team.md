# project Red Team

**Zadanie 1 - Łamanie haseł (met. 
brute-force) 1/3**


1) `81dc9bdb52d04dc20036dbd8313ed055` - wynik: 1234(MD5)
2)`d8826bbd80b4233b7522d1c538aeaf66c64e25a`  wynik: 4121(sha1)
3)`b021d0862bc76b0995927902ec697d97b5080341a53cd90b780f50fd5886f4160bbb9d4a573b76c23004c9b3a44ac95cfde45399e3357d1f651b556dfbd0d58f` wynik: 6969 (sha512)
4)`31bca02094eb78126a517b206a88c73cfa9ec6f704c7030d18212cace820f025f00bf0ea68dbf3f3a5436ca63b53bf7bf80ad8d5de7d8359d0b7fed9dbc3ab99`      wynik: 0  (sha512)



**Zadanie 1 - Łamanie haseł (met. 
brute-force) 2/3**

1)`9e66d646cfb6c84d06a42ee1975ffaae90352bd016da18f51721e2042d9067dcb120accc574105b43139b6c9c887dda8202eff20cc4b98bad7b3be1e471b3aa5`  wynik: sda  (sha512)
2`)8a04bd2d079ee38f1af784317c4e2442625518780ccff3213feb2e207d2be42ca0760fd8476184a004b71bcb5841db5cd0a546b9b8870f1cafee57991077c4a9`  wynik: Asia  (sha512)
 

**Zadanie 1 - Łamanie haseł (met. 
brute-force) 3/3**

`44d9886c0a57ddbfdb31aa936bd498bf2ab70f741ee47047851e768db953fc4e43f92be953e205a3d1b3ab752ed90379444b651b582b0bc209a739a624e109da`
wynik: TO^^EK  (sha512)

hashcat -a 3 -m 1700 -w 3 hash.txt "?a?a?a?a?a?a" /home/kali/Desktop/rockyou.txt


**Zadanie 2 - Łamanie haseł (met. 
słownikowa) 1/2**

1)`9fd8301ac24fb88e65d9d7cd1dd1b1ec`       wynik:	butterfly(MD5)
2)`7f9a6871b86f40c330132c4fc42cda59`  
wynik: tinkerbell(MD5)
3)`6104df369888589d6dbea304b59a32d4`	
wynik: blink182(MD5)
4)`276f8db0b86edaa7fc805516c852c889` 
wynik: baseball(MD5)
5)`04dac8afe0ca501587bad66f6b5ce5ad`  
wynik: hellokitty(MD5)



**Zadanie 2 - Łamanie haseł (met. 
słownikowa) 2/2**

1)`7ab6888935567386376037e042524d27fc8a24ef87b1944449f6a0179991dbdbc481e98db4e70f6df0e04d1a69d8e7101d881379cf1966c992100389da7f3e9a`  
wynik: spiderman (sha512) 
hashcat -m 1700 hash.txt /home/kali/Desktop/rockyou.txt
2)`470c62e301c771f12d91a242efbd41c5e467cba7419c664f784dbc8a20820abaf6ed43e09b0cda994824f14425db3e6d525a7aafa5d093a6a5f6bf7e3ec25dfa` 
wynik: rockstar(sha512)


**zadanie3**
Urochomienie wireshark
logowanie na stronie  http://testphp.vulnweb.com/login.php jako "admin" z hasłem "password"
zatrzymanie wiresharka
ustałamy filtr "http" i szukamy pakietu login
Dalej szukamy "tcp stream" pakietu
i widzimy dane logowania

**zadanie 4** 

ssh uranus@10.0.2.12
echo "password1" > sekret1.txt
echo "password2" > sekret2.txt
ftp 10.0.2.4
sudo systemctl retart vsftpd


**zadanie 5**
echo "haslo" > haslo.txt
echo "password1" > sekret1.txt
echo "password2" > sekret2.txt
put haslo.txt
get sekret1.txt
get sekret2.txt






### Zadanie 1
### Slajd 1
### 1)  
***Hasło***
81dc9bdb52d04dc20036dbd8313ed055
***Narzędzie*** 
https://md5hashing.net/hash/md5/81dc9bdb52d04dc20036dbd8313ed055
***Typ algorytmu*** 
Md5
***Wynik***
1234

### 2)  
***Hasło***
d8826bbd80b4233b7522d1c538aeaf66c64e259a
***Narzędzie*** 
https://md5hashing.net/hash/md5/81dc9bdb52d04dc20036dbd8313ed055
***Typ algorytmu*** 
Fnv1a52
***Wynik***
4121

### 3)  
***Hasło***
b021d0862bc76b0995927902ec697d97b5080341a53cd90b780f50fd5886f4160bbb9d4a573b76c23004c9b3a44ac95cfde45399e3357d1f651b556dfbd0d58f
***Narzędzie*** 
https://md5calc.com/hash/sha512/6969
***Typ algorytmu*** 
SHA512
***Wynik***
6969


![zadanie1_numer3.jpg](../_resources/zadanie1_numer3.jpg)


### 4)  
***Hasło***
31bca02094eb78126a517b206a88c73cfa9ec6f704c7030d18212cace820f025f00bf0ea68dbf3f3a5436ca63b53bf7bf80ad8d5de7d8359d0b7fed9dbc3ab99
***Narzędzie*** 
https://crackstation.net/
***Typ algorytmu*** 
sha512
***Wynik***
0


![zadanie1_numer4.jpg](../_resources/zadanie1_numer4.jpg)



### 1)  
***Hasło***
9e66d646cfb6c84d06a42ee1975ffaae90352bd016da18f51721e2042d9067dcb120accc574105b43139b6c9c887dda8202eff20cc4b98bad7b3be1e471b3aa5
***Narzędzie*** 
https://crackstation.net/
***Typ algorytmu*** 
sha512
***Wynik***
sda

### 2)  
***Hasło***
9e66d646cfb6c84d06a42ee1975ffaae90352bd016da18f51721e2042d9067dcb120accc574105b43139b6c9c887dda8202eff20cc4b98bad7b3be1e471b3aa5
***Narzędzie*** 
https://crackstation.net/
***Typ algorytmu*** 
sha512
***Wynik***
Asia


### Zadanie 1 - Łamanie haseł (met. 
brute-force) 3/3

44d9886c0a57ddbfdb31aa936bd498bf2ab70f741ee47047851e768db953fc4e43f92be953
e205a3d1b3ab752ed90379444b651b582b0bc209a739a624e109da
TO^^EK 
(sha512)

hashcat -a 3 -m 1700 -w 3 hash.txt "?a?a?a?a?a?a" /home/kali/Desktop/rockyou.txt

![maxspeed.jpg](../_resources/maxspeed.jpg)



![zadanie1.3_hashcat.jpg](../_resources/zadanie1.3_hashcat.jpg)

**Zadanie 2 - Łamanie haseł (met. 
słownikowa) 2/2**

### 1)`7ab6888935567386376037e042524d27fc8a24ef87b1944449f6a0179991dbdbc481e98db4e70f6df0e04d1a69d8e7101d881379cf1966c992100389da7f3e9a`  
wynik: spiderman (sha512) 
hashcat -m 1700 hash.txt /home/kali/Desktop/rockyou.txt
### 2)`470c62e301c771f12d91a242efbd41c5e467cba7419c664f784dbc8a20820abaf6ed43e09b0cda994824f14425db3e6d525a7aafa5d093a6a5f6bf7e3ec25dfa` 
wynik: rockstar(sha512)
hashcat -m 1700 hash.txt /home/kali/Desktop/rockyou.txt


### **zadanie3**
Urochomienie wireshark
logowanie na stronie  http://testphp.vulnweb.com/login.php jako "admin" z hasłem "password"
zatrzymanie wiresharka
ustałamy filtr "http" i szukamy pakietu login
Dalej szukamy "tcp stream" pakietu
i widzimy dane logowania

![zadanie3.1.jpg](../_resources/zadanie3.1.jpg)



![zadanie3.0.1.jpg](../_resources/zadanie3.0.1.jpg)



![zadanie3.0.2.jpg](../_resources/zadanie3.0.2.jpg)



### **zadanie 4** 
**logowanie do maszyny SDA:**
ssh uranus@10.0.2.12
sudo nano /etc/vsftpd.conf (plik który konfigurujemy)
sudo systemctl retart vsftpd
**poniższe polecenia wykonujemy na kalim:**
echo "password1" > sekret1.txt
echo "password2" > sekret2.txt
ftp 10.0.2.12
put sekret1.txt
put sekret2.txt

![zadanie4.jpg](../_resources/zadanie4.jpg)



![zadanie4.3.jpg](../_resources/zadanie4.3.jpg)



![zadanie4.5.jpg](../_resources/zadanie4.5.jpg)



![zadanie 4.6.jpg](../_resources/zadanie 4.6.jpg)



![zadanie4.7.jpg](../_resources/zadanie4.7.jpg)


### **Zadanie 5**
echo "haslo" > haslo.txt
ftp 10.0.2.12
put haslo.txt
get sekret1.txt
get sekret2.txt


![zadanie 5.jpg](../_resources/zadanie 5.jpg)



![zadanie 5.1.jpg](../_resources/zadanie 5.1.jpg)



### **Zadanie 6 - Eternal Blue** 
Użyjemy maszny wirtualnej z platformy "tryhackme"

https://tryhackme.com/room/blue
Rekonesans za pomocą nmap 
Ustalamy że windows jest podatny na "ETERNAL BLUE"
![zadanie6.1.jpg](../_resources/zadanie6.1.jpg)



wyszukujemy exploit w metasploicie
![zadanie6.2.jpg](../_resources/zadanie6.2.jpg)


Ustawiamy opcje "RHOSTS" i "LHOST"


![zadanie6.3.jpg](../_resources/zadanie6.3.jpg)

Uruchamiamy exploit


![zadanie6.4.jpg](../_resources/zadanie6.4.jpg)

zmieniamy shella na "meterpreter"

![zadanie6.5.jpg](../_resources/zadanie6.5.jpg)


![zadanie6.6.jpg](../_resources/zadanie6.6.jpg)

zmieniamy process

![zadanie6.7.jpg](../_resources/zadanie6.7.jpg)

za pomocą polecenia "hashdump" wyciągamy hash dla
użytkownika  Jon



![zadanie6.8.jpg](../_resources/zadanie6.8.jpg)


crakujemy haslo

![zadanie6.9.jpg](../_resources/zadanie6.9.jpg)

**flagi**


![zadanie6.10.jpg](../_resources/zadanie6.10.jpg)



![zadanie6_flagi_1_i_2.jpg](../_resources/zadanie6_flagi_1_i_2.jpg)



![zadanie6_flaga_3.jpg](../_resources/zadanie6_flaga_3.jpg)



![zadanie6.final.jpg](../_resources/zadanie6.final.jpg)


