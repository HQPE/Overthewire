
Natas6 sayfasında, içine bir "secret" girip göndereceğin bir form var. Doğru secret’i bilmiyorsun.

<img width="1146" height="815" alt="image" src="https://github.com/user-attachments/assets/dd0ac476-2cc0-4d71-8d01-bf246272a02b" />

secret değişkeni, includes/secret.inc dosyasından dahil ediliyor.

Eğer POST ile gönderdiğimiz secret bu değişkene eşitse, Natas7 şifresini alıyoruz

<img width="1234" height="700" alt="image" src="https://github.com/user-attachments/assets/af85a7f1-b4f3-43d6-bd9e-4fd687aa4595" />
includes/secret.inc dosyasına doğrudan web tarayıcıdan erişmeyi dene:

text
http://natas6.natas.labs.overthewire.org/includes/secret.inc
Bu dosya düz metin olarak görüntülenebilir (çünkü .inc uzantısı genelde PHP olarak işlenmez, kaynak kodu açar).

<img width="1113" height="338" alt="image" src="https://github.com/user-attachments/assets/aeef321c-c706-4c98-bc13-7f5c8411ab6c" />

Ana sayfaya dön (http://natas6.natas.labs.overthewire.org).

Input kutusuna FOETUNGHFEEUHOFUOTU yaz.

Submit Query butonuna tıkla.

<img width="846" height="541" alt="image" src="https://github.com/user-attachments/assets/a8a0e147-26db-49ba-8d98-84bc39b5660c" />
