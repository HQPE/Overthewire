Natas8 sayfasında, içine bir "secret" girip göndereceğin bir form var. Doğru secret'i bilmiyorsun.

<img width="812" height="626" alt="image" src="https://github.com/user-attachments/assets/8dd5bed1-8d95-4ca4-a5ad-0a4711ed8fda" />

Sayfadaki "View sourcecode" bağlantısına tıkla. Kaynak kodunda şu PHP kodu var:

<img width="1183" height="772" alt="image" src="https://github.com/user-attachments/assets/a2718687-b618-414c-abd7-91787e49bb3b" />

Anladığımız:

encodeSecret() fonksiyonu şu işlemleri yapıyor:

base64_encode($secret) → Secret'i Base64'e çevir
strrev() → Base64 stringini ters çevir
bin2hex() → Ters çevrilmiş string'i hex'e çevir
$encodedSecret = "3d3d516343746dd4d6d6c31566956362" bizim hedefimiz.

<img width="1541" height="480" alt="image" src="https://github.com/user-attachments/assets/a98f4a45-e32d-406b-a90e-b13d92d3302c" />

Doğru secret'i bulmak için encoding işlemini tersine çevirmeliyiz:

Hex → String: 3d3d516343746dd4d6d6c31566956362 → normal metne çevir

String'i ters çevir (rev)

Base64 decode et

Sonuç: oubWYf2kBq

Ana sayfaya dön (http://natas8.natas.labs.overthewire.org)

Input kutusuna oubWYf2kBq yaz

Submit Query butonuna tıkla

<img width="762" height="551" alt="image" src="https://github.com/user-attachments/assets/4877e4b6-0d8d-4dc4-91c3-e74aa8973bdb" />
