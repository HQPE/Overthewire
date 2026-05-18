Sistem, page parametresini hiçbir filtreleme yapmadan include() fonksiyonuna aktarıyor. Bu sayede, sadece home veya about dosyalarını değil, sistemdeki diğer dosyaları da okumayı deneyebilirsiniz.

Hedefimiz, bir sonraki seviye olan natas8 için şifrenin saklandığı dosyaya ulaşmak. OverTheWire'da tüm seviyelerin şifreleri, /etc/natas_webpass/ dizini altında, ilgili seviyenin ismiyle (natas8) tutulur.

Salıdırıyı Gerçekleştirin: Adres çubuğundaki page= parametresinin değerini, hedef dosyanın yolunu gösterecek şekilde değiştirin ve enter'a basın.
http://natas7.natas.labs.overthewire.org/index.php?page=/etc/natas_webpass/natas8

Eğer her şey doğru gittiyse, sayfada size bir sonraki seviyenin şifresini gösterecektir.

<img width="937" height="570" alt="image" src="https://github.com/user-attachments/assets/f55b1f35-5aa3-4292-acc1-6c96365cb12f" />
