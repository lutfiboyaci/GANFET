# HAFTALIK PLANLAR
## 18.12.2017-24.12.2017
1. Fizik bölümünde Bilge Demirköz Hoca ve ekibinden 3 kişi ile bir toplantı yaptık. Toplantı notlarını ayrı bir doküman olarak paylaşacağım. 
2. 3 ve 5. Entegreler Vref sinyali olarak 8V üretiyordu. Doğal olarak GANFET'lere (3. ve 5.) ulaşan Vgs sinyali de bu seviyede oluyordu. GANFETLER (3. ve 5.) zarar görmüş olabilir. 4. ve 6. Driver IC de yanmıştı. 
3. 3-4-5-6 kanaldaki Driver IC ve GANFET'leri toptan değiştirdik. Bu işlem zor bir iş. paketler QFN ve BGA olduğu için işlemler zor ve ardından Xray görüntülemesi gerektiriyor. 
4. 1 ve 2. kanal anahtarlamasına rağmen, Vgs sinyali okuma çalışmıyordu. muhtemelen RC time constant büyük geliyor. 1Mohm direnç bölücü 5. dirençler 100Kohm'lar ile değiştirildi. 
Değişikliklerden sonra testleri yaptım. Driver IC'lerde yine benzer sorunlar oluştu. 4. IC yine ısındı. Demek ki problem IC'lerde değil, başka bir şeyde. Vgs okuma bu sefer daha iyi çalıştı. Dirençlerin 10kOhm'a düşürülmesiyle tamamen çözülecektir diye tahmin ediyorum. Test sonuçlarını paylaşacağım.
## 11.12.2017-17.12.2017
1. Akım okuma devresi çalışmıyordu, problemin akım okuma entegresinin yerinden kaynaklandığını düşünüyorum. İlk üretimde 50V'dan Grounda doğru Taş Direnç, Akım okuma, GANFET şeklinde sıralanıyordu. GANFET ON durumunda Drain gerilimini 0V'a çektiğinde Akım okuma entegresi pini de 0V'u görüyor. Entegre dışardan besleme almadığı için gücünü bu pinden alıyor. 0V durumunda güç alamadığı için çalışmıyor olabilir. 
2. Akım okuma devresinin yerini değiştirdik. 50V'dan Grounda doğru Akım okuma, Taş direnç, GANFET şeklinde sıralandı. GANFET ON durumunda Drain gerilimini 0V'a düşürünce, 50 Volt taş direnç üzerine binecek ve akım okuma entegresi hep 50'u görecek. 
3. Revizyon yapıldıktan sonra testi yaptım. Problem tahmin ettiğim gibi çözüldü. İlgili osiloskop görüntülerini paylaşacağım.
## 20.11.2017-10.12.2017
1. GAN_RAD_TEST_KARTI dizgisi tamamlandı.
2. Alüminyum şase üzerine 6 adet taş direncin yerleştirilip ısının atılacağı bir heatsink üretildi. 
3. Kartı denedim. Kare dalga üretimi başarılı. 
4. 6 adet kanaldan yalnızca 1. ve 2. kanal anahtarlıyor. 3. ve 5. kanal Driver IC'lerin Vref pininde 5V üretmesi gerekirken 8V civarında üretiyor. Doğal olarak GANFET'lerin Vgs Sinyali de 8V olarak gidiyor. Bu EPC GANFET'lerin Vgs max sınırı dışında. GANFET 3 ve 5 yanmış olabilir. 4. ve 6. driver'a termal kamera ile bakınca 110 C'ye ulaştıklarını gördüm. Driver IC 4 ve 6 yandı. değiştirilmesi gerekiyor. 
5. Akım okuma devresi çalışmıyor. GANFET Turn-ON olduğunda AD8212 Akım okuma entegresinin güç aldığı pin 0 V'a düşüyor. Problem buradan kaynaklanıyor diye tahmin ediyorum. akım okuma entegresini 50V girişine taşımak gerekiyor. Böylece V+ pini hep 50V'u görecek. Bunu yapmak problemi çözebilir.
6. GANFET'in Vgs gerilimini direnç bölücü üzerinden okuyoruz. Fakat düzgün okuyamıyoruz. Direnç bölücü direnç değerleri çok yüksek olduğu için Vgs sinyali hızına yetişemiyor. RC time constant çok yüksek. Direnç değerlerinin düşürülmesi problemi çözebilir.
7. Laboratuvar test çalışmaları yapıldı. Gerekli gördüğüm osiloskop görüntülerini paylaşacağım.
## 06.11.2017-12.11.2017
Kazıma kart üretimi gerçekleştirildi. 
Kartın tamamlanması için benim yapacağım kısım bitmiş oldu. Üretim için sıraya girdi kart. 
Yarın entegrasyon grubu ile detayları konuşacağım, kartın dizgisini önümüzdeki hafta bitirmeyi planladıklarını söylediler. 

## 30.10.2017-03.11.2017
depo malzemesinde 1 eksik malzeme vardı-1n5401 PNP transistör. satınalma süreçleri uzun olacağı için Ulus konya sokaktan aldım. 
SAP sistemine geçildiği için, malzeme kodları SAP sisteminde güncellendi ve buna göre yeni kodlar alınarak malzemeler istendi. 

## 23.10.2017-29.10.2017
Üretim Dosyaları tamamlanacak. 
ilgili KİT açılacak. 
Depo malzemeleri istenecek.

## 16.10.2017-20.10.2017
PCB Layout tasarımı tamamlandı. Üretim dosyaları oluşturmak için gereken yeni program öğrenildi.

## 09.10.2017-15.10.2017
PCB Layout tasarımı devam etti.

## 25.09.2017-01.10.2017
1.PCB Tasarımı başlatılacak, ilerlenecek.

## 18.09.2017-22.09.2017
1. Şematik çizimi bitecek.
2. ilgili makaleler okumaya devam edilecek.

Şematik 90% bitti

## 11.09.2017-17.09.2017
1. Radyasyon testi için ilgili ekiple yaptığımız toplantıda test düzeneği ayrıntılarını, takvimi, detayları konuştuk. Önce proton parçacıklı SEE yapmayı planlıyoruz. Atom Enerjisi kurumunda, Bilge Hoca'nın proton hızlandırma labında.  Burada run-time ölçümler alacağız. buna uygun bir şematik ve PCB tasarlamak lazım.  6x8 cm lik bir alana test edilecek malzemeleri sıkıştırmam gerekiyor. 
2. Bu ayrıntılara göre şematik çizimi ve PCB'yi tekrar planladım.
3. Radyasyon tesleri, etkileri ile ilgili okumalar yapıyorum. Mendeley'e paylaşıyorum. 

## 05.09.2017-10.09.2017
### Plan:
1. Radyasyon testi devresi şematik çizimi bitirilecek
2. Şematik çiziminden sonra zaman kalırsa PCB tasarımına geçilecek

şematik çizimi bitirilemedi. test için ilgili ekiple konuşmamdan sonra iş düşündüğümden daha ayrıntılı çıktı. haftaya detayların konuşulacağı bir toplantı düzenledik. 

## 05.06.2017-11.06.2017
### Plan:
1. 2 numaralı sürücü devresi turn off süresini düşürmek için gate direnci daha düşük bir direnç ile değiştirildikten sonra, tekrar test edilecek. sonuçlar gözlenecek. Math fonksiyonu ile osiloskopta loss grafiği çizdirilecek.
2. 1 numaralı sürücü devresi test edilecek.

planlar gerçekleştirildi

## 29.05.2017-02.06.2017
### Plan:
1. 2 numaralı sürücü devresi test edilecek

planlar gerçekleştirildi, test sonuçları paylaşıldı



## 22.05.2017-28.05.2017
1. Timer entegresi test edildi. Duty Sinyali üretildi. 
2. Sinyalin FET'e iletimini sağlayacak jumper lehimlemesi için ilgili teknisyene iletilerek lehimleme yapıldı.



## 15.05.2017-21.05.2017
### Kart üretimi gerçekleşti, Ganların X-ray cihazında kısa devre açık devre hatası olup olmadığı kontrol edildi.


## 08.05.2017-14.05.2017
### Plan:
1. Ganların lehimi ayrı yapılıyormuş. LGA paket olduğu için normal lehimleme değil fırınlama yapılması gerekiyormuş. Her teknisyen yapamadığı için, iş ilk atanan teknisyenden alınıp fırınlamayı yapabilecek teknisyene aktarıldı. Kartın üretimini bekliyoruz.
2. Devrede kullanılan malzemelerle ilgili (timer, sürücü entegreleri) simulasyonlar yapılacak. Çıktılar eklenecek.

planlar gerçekleştrildi.

# HAFTALIK PLANLAR
## 24.04.2017-28.04.2017
### Plan:
1. Kartın üretimi LPKF (kazıma kart) cihazında gerçekleştirilecek.
2. Madde 1 gerçekleşirse, Kart dizimi talebi açılarak ilgili teknisyen ataması yapılacak. 
3. Madde 2 gerçekleşirse (uygun olan teknisyen var ise), depodan talep edilen malzemeler teknisyene iletilerek, dizim işlemi başlatılacak.

Planlar gerçekleştirildi


## 21.04.2017-23.04.2017
### Plan:
1. Depodan talep edilmeyen son malzemeler talep edilecek, talep işi bitecek. 
2. Kart baskısı için output dosyaları hazırlanacak.(Gerber ve Drill files)   (dosyaları kontrol etmeyi unutma)
3. Malzeme dizimi için BoM dosyası ve malzeme yerleşimi dosyası hazırlanacak. 

Planlar gerçekleştirildi.


## 10.04.2017-14.04.2017
### Plan:

* "eGAN FET Drivers (EPC)"
* "Printed Circuit Board Layout and Probing for GaN Power Switches. (Transphorm)"
* "Investigation of Driver Circuits for GaN HEMTs in Leaded Packages (Transphorm)"

1. Makaleleri okunacak, PCB layouta yön verecek çıkarımlar yapılacak, çıkarımlara göre PCB'ye son hali verilecek.
2. PCB'de kullanılacak malzemelerden elimde olanlar için malzeme tanımları yapılarak depo kodları oluşturulacak. Malzemeler depoya teslim edilecek, depodaki malzemeler talep edilecek.
3. Schematic malzeme kodları depo kodları ile eşletirilecek. 
4. PCB üretimi için KİT tanımlanacak.

1-3-4 maddeleri gerçekleştirildi.  
2. madde: malzemeler teslim edildi, depo girişleri gerçekleşmediği için talep gerçekleştirilemedi.


