# Akilli-Sera-Otomasyonu
KULLANILAN TEKNOLOJİLER

 . NODEMCU Development Kit
 
 . BLYNK
 
 . UBIDOTS BULUT PLATFORMU
 
 . DHT11 Sıcaklık Sensörü
 
 . Toprak Nem Sensörü
 
 . Su pompası 
 
 . Soğutucu Fan
 
 . Güç Kaynağı - 9V Pil
 
 
SİSTEMİN ÇALIŞMA PRENSİBİ

  Sera otomasyon sistemi NODEMCU Mikrodenetleyici kartıyla tasarlanmıştır. Sistemde toprak nem sensörü ve DHT11 sıcaklık ve nem sensörü bulunmaktadır. Sensörlerden gelen verilere göre su pompası ve fan aktüatörleri çalışıp kapanmaktadır.
  
 Bu projede UBIDOTS bulut bilişim alt yapısını kullanarak sensörlerden gelen seranın sıcaklık, nem ve toprağın nem değerlerini bulut üzerinde bir database’e kaydedip bu değerleri tablo veya grafiksel bir şekilde görüp belirtilen değerler aşıldığında kullanıcıya mobil uygulama olan BLYNK platformu üzerinden bilgilendirme mesajlarının gönderilip sistemde belirtilen işlemlerin otomatik olarak gerçekleştirilmesi sağlanmıştır.
 
  Sistemde toprak sulaması; toprağın içine konumlandırılmış toprak nem sensörü topraktaki nem durumuna göre NODEMCU’ya analog verileri gönderir. NODEMCU’ da denetlenen veriler istenilen değer aralığının altında ise sulama sistemine aktif olması komutu vererek su pompasını çalıştırır. Sistemi istenilen değer aralığına getirir ve belli bir süre bu seviyede çalıştıktan sonra su pompasını devre dışı bırakır. Toprak sulama sistemi aşamasında BLYNK mobil uygulamasında toprağın nem durumu düşük iken “Toprağınızı sulayın!” bildirimi kullanıcıya gönderilir. Bildirim gönderildikten sonra su pompası devreye girip toprak nem durumu belirlenen seviyeye ulaştığında is “Sulama gerçekleştirildi! Toprağınız nemli :D” bildirimi kullanıcıya gönderilir.
  
  Seranın ortam sıcaklığı; seranın merkezi bir bölgesine konumlandırılan sıcaklık ve nem sensörü ortamda sıcaklığı ölçüp verileri NODEMCU’ya gönderir. Her bitkinin optimum yetişme sıcaklığı farklıdır ve bu sebepten ortam sıcaklığını belli aralıklarda tutmak çok önemlidir. Sistem içinde sıcaklığın artması sonucu fan ile havalandırma sistemi aktif edilerek ortam sıcaklığı istenilen seviyeye çekilmiş olur.

