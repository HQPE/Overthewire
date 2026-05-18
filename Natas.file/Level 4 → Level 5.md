Natas4 sayfasına giriş yaptığında aşağıdaki gibi bir hata alırsın:

Access disallowed. You are visiting from "" while authorized users should come only from "http://natas5.natas.labs.overthewire.org/"

<img width="1137" height="671" alt="image" src="https://github.com/user-attachments/assets/6ef7fcd0-449a-4ed5-ad7f-6661c5d32fe1" />

Sebep:
Sunucu, isteğin hangi web sitesinden geldiğini kontrol eden HTTP Referer başlığını denetliyor. İstek boş ("") veya yanlış geldiği için erişim engelleniyor.

Çözüm (Burp Suite ile):

Burp Suite Proxy’yi aç ve tarayıcını Burp’e yönlendir.

Sayfayı yenile ve HTTP isteğini yakala (Intercept on).

İsteği Repeater’a gönder (Ctrl+R).

İsteğe aşağıdaki satırı ekle veya değiştir:

<img width="1356" height="846" alt="image" src="https://github.com/user-attachments/assets/04bad150-04b2-4f17-835f-af1c59193f0d" />


– burada istek ve cevap görülüyor. Cevap içinde Access granted. The password for natas5 is ... yazıyor.)

Sonuç:
Sunucu, geçerli Referer başlığını görünce erişim izni verir ve Natas5 şifresini döndürür:
