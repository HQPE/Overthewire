Natas5 sayfasına giriş yaptığında şu hatayı alırsın:

Access disallowed. You are not logged in


<img width="847" height="671" alt="image" src="https://github.com/user-attachments/assets/6cb26ecc-6a7c-4913-9fe6-43b2b65a55fe" />
Sebep:
Sunucu, kullanıcının giriş yapıp yapmadığını bir cookie (loggedin) üzerinden kontrol ediyor. Varsayılan değeri 0 olduğu için sistem seni oturum açmamış sayıyor.

Çözüm (Geliştirici Araçları ile):

Tarayıcıda Geliştirici Araçları’nı aç (F12).

Storage (Firefox) veya Application (Chrome) sekmesine git.

Cookies → https://natas5.natas.labs.overthewire.org kısmını bul.

loggedin isimli cookie’yi gör. Değeri 0 olacak.

Bu değeri çift tıkla, 0’ı sil ve yerine 1 yaz. Enter’a bas.
(Görsel 2’nin alt kısmında loggedin_1 olarak görünüyor, doğru değer loggedin=1 olmalı.)

Sayfayı yenile (F5 veya Ctrl+R).



Sonuç:
Cookie loggedin=1 olduğunda sunucu seni giriş yapmış kabul eder ve ekrana Natas6 şifresini yazdırır.
<img width="1322" height="752" alt="image" src="https://github.com/user-attachments/assets/cccd1503-21c9-4963-850f-8afa364dd772" />
