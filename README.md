# AI Network Optimizer- Yapay Zeka Destekli Kendini Optimize Eden Ağ

Proactive AI Network Agent telekomünikasyon erişim ağlarında yaşanan performans problemlerini kullanıcıyı etkilemeden önce tespit etmeyi amaçlayan, 
yapay zekâ destekli proaktif bir AIOps sistemidir.

## Amaç ve Problem Tanımı
Günümüzde telekomünikasyon ağlarında yaşanan performans problemleri, çoğunlukla kullanıcı şikâyetleri sonrasında fark edilmekte ve bu durum reaktif bir arıza yönetim sürecine yol açmaktadır. Bu yaklaşım, ortalama çözüm süresinin uzamasına, gereksiz saha müdahalelerine ve müşteri memnuniyetinin azalmasına neden olmaktadır. Proactive AI Network Agent projesinin amacı, ağ performans verilerini sürekli izleyerek olasılıklı sorunları kullanıcıyı etkilemeden önce tespit etmek, bireysel ve kitlesel problemleri ayırt edebilmek ve uygun operasyonel aksiyonların proaktif olarak alınmasını sağlamaktır.

## Sistem Mimarisi ve Çalışma Mantığı

AI Network Optimizer, ağ durumunu senaryo tabanlı olarak analiz eden, metrikleri yorumlayan ve sonuçları kullanıcıya sade bir arayüzle sunan bir demo sistemidir.
Sistem temel olarak şu akışla çalışır:
1-Kullanıcı bir Demo Senaryosu seçer
2-Seçilen senaryoya ait ağ metrikleri simüle edilir
3-Metrikler eşik değerlerle karşılaştırılır
4-Genel durum belirlenir (Sağlıklı / Dikkat / Kritik)
5-AI Tanı Sistemi devreye girerek metinsel analiz üretir
6-Uygulanabilir Önerilen Aksiyonlar sunulur
  Bu yapı, gerçek bir ağ izleme sisteminin sadeleştirilmiş bir temsilidir.

## Demo Senaryoları
Uygulama, farklı ağ problemlerini temsil eden ön tanımlı senaryolar içerir. Her senaryo, farklı metrik değerleri ve farklı sonuç ekranları üretir.

Desteklenen senaryolar:
-İnternet Normal: Sağlıklı bağlantı, düşük ping, sıfıra yakın paket kaybı
-Yavaş WiFi: Düşük hızlar, orta seviye gecikme
-Modem Sorunu: Dalgalı hızlar, yüksek ping, paket kaybı
-Altyapı Arızası: Çok düşük hızlar veya bağlantı kopması
-Ağ Yoğunluğu: Trafik kaynaklı gecikmeler
-Kesinti: Ağın tamamen veya neredeyse tamamen kullanılamaz olması

Bu senaryolar, kullanıcıya farklı problemlerin sistem tarafından nasıl yorumlandığını göstermeyi amaçlar.

## Gerçek Zamanlı Ağ Metrikleri
Her senaryo için aşağıdaki temel metrikler hesaplanır ve gösterilir:
-İndirme Hızı (Mbps)
-Yükleme Hızı (Mbps)
-Ping (Gecikme – ms)
-Paket Kaybı (%)

Metrikler, kullanıcı deneyimini artırmak amacıyla renk kodları ile sunulur:
-Yeşil: Normal değerler
-Sarı: Kabul edilebilir fakat dikkat edilmesi gereken durum
-Kırmızı: Kritik seviye
    Bu sayede kullanıcı, teknik bilgiye sahip olmasa bile bağlantı durumunu hızlıca anlayabilir.

## Durum Tespiti ve Uyarı Mekanizması
Sistem, metrikleri analiz ederek genel bir durum mesajı üretir:
-Bağlantı Sağlıklı
-Dikkat Gerekli
-Sorun Tespit Edildi
    Bu uyarılar, ağ kalitesinin genel özetini tek bir bakışta sunar ve kullanıcının hangi seviyede müdahale etmesi gerektiğini açıkça belirtir.

## AI Tanı Sistemi
AI Tanı Sistemi, ağ metriklerini birlikte değerlendirerek problemin olası kaynağını belirlemeye çalışır.
Örnek çıkarımlar:
-Sorunun modem veya kullanıcı cihazından kaynaklanması
-Altyapı tarafında bir problem bulunmaması
-Yüksek ping ve paket kaybının performansı düşürmesi
-Bazı demo senaryolarında, harici AI servisinin yanıt veremediği durumlar da özellikle gösterilerek hata yönetimi senaryosu simüle edilmiştir.

## Önerilen Aksiyonlar
Tanı sonucuna göre sistem, kullanıcıya uygulanabilir öneriler sunar:
-WiFi yerine Ethernet kablosu kullanılması
-Modem firmware güncellemesinin kontrol edilmesi
-Modemin yeniden başlatılması
-Sorun devam ederse donanım değişimi önerisi
-Herhangi bir sorun yoksa bilgilendirici mesajlar
    Bu bölüm, kullanıcının ne yapması gerektiğini net ve sade şekilde anlamasını sağlar.

## Demo Kapsamı ve Sınırlamalar
Bu proje bir demo uygulamasıdır. Tüm ağ verileri simüle edilmiştir Gerçek ağ ölçümü yapılmaz. Amaç, arayüz, analiz mantığı ve kullanıcı deneyimini göstermektir

## Sonuç
AI Network Optimizer, yapay zeka destekli ağ izleme ve problem tanılama sistemlerinin nasıl çalışabileceğini gösteren modern bir demo arayüzüdür.
Proje; Eğitim, Sunum, Kavramsal prototip amaçları için tasarlanmıştır.

