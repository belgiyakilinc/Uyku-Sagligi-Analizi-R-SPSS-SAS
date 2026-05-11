# Uyku Sağlığı ve Yaşam Tarzı: Çok Değişkenli İstatistiksel Analiz (R, SPSS, SAS)

Bu proje, "Sleep Health and Lifestyle Dataset" kullanılarak bireylerin uyku düzenleri ve yaşam tarzı alışkanlıkları arasındaki karmaşık ilişkileri inceleyen kapsamlı bir istatistiksel analiz çalışmasıdır. Çalışma kapsamında R, SPSS ve SAS yazılımları entegre bir şekilde kullanılmış ve çok değişkenli istatistiksel yöntemler uygulanmıştır.

## 📊 Veri Seti Hakkında
Veri seti, 374 bireye ait uyku süresi, uyku kalitesi, fiziksel aktivite seviyesi, stres düzeyi, kalp atış hızı, günlük adım sayısı ve uyku bozukluğu durumu (Yok, İnsomnia, Uyku Apnesi) gibi 13 farklı değişkeni içermektedir. 

## 📁 Proje Dosya Yapısı
Depo içerisindeki analizler yöntemlerine göre aşağıdaki klasörlere ayrılmıştır:

* `Veri_Analizi/`: Değişkenlerin temel betimsel istatistikleri, çarpıklık/basıklık incelemeleri ve normallik testleri.
* `manova_analizi/`: Uyku bozukluğu türlerinin, uyku süresi ve kalitesi üzerindeki ortak etkisini inceleyen Çok Değişkenli Varyans Analizi kodları ve grafikleri.
* `faktor_analizi/`: Veri setindeki gizli yapıyı ortaya çıkarmak için yapılan Temel Bileşenler ve Faktör Analizi uygulamaları.
* `diskriminant_analizi/`: Bireylerin yaş, aktivite, uyku süresi ve kalitesine dayanarak hangi uyku bozukluğu grubuna ait olduklarını tahmin eden sınıflandırma modeli.
* `logistik_regresyon_analizi/`: Uyku bozukluğu (Apne/İnsomnia) risk faktörlerini (yaş, stres, kalp atış hızı vb.) belirlemek için kurulan çok terimli lojistik regresyon modeli.
* `kümeleme_analizi/`: Bireyleri sağlık ve yaşam tarzı benzerliklerine göre gruplara ayıran hiyerarşik ve k-ortalamalar (k-means) kümeleme analizi algoritmaları.
* `Analiz_Sonuc_Raporu.pdf`: Tüm analiz çıktılarının, varsayım kontrollerinin ve istatistiksel yorumların bulunduğu detaylı final raporu.

## 📈 Temel Bulgular
Yapılan analizler sonucunda elde edilen başlıca istatistiksel bulgular şunlardır:

* **MANOVA:** Uyku bozukluğu (Özellikle Uyku Apnesi), bireylerin uyku süresi ve kalitesini istatistiksel olarak anlamlı düzeyde düşürmektedir (p < 0.001). Ayrıca uyku apnesi yaş ile pozitif bir korelasyon göstermektedir.
* **Lojistik Regresyon:** Uyku kalitesindeki düşüş, stres seviyesindeki artış ve yaşın ilerlemesi, uyku apnesi ve insomnia riskini anlamlı şekilde artırmaktadır. Modelin genel sınıflandırma başarısı oldukça yüksektir (Örn: Uyku problemi olmayanları %93,2 oranında doğru tahmin etmiştir).
* **Diskriminant Analizi:** Kurulan diskriminant fonksiyonları ile hastaların uyku bozukluğu grupları çapraz doğrulama (cross-validation) sonucunda %83,2 doğruluk oranıyla sınıflandırılmıştır.
* **Faktör ve Kümeleme Analizleri:** Faktör analizi öncesi KMO değeri 0.783 olarak bulunmuş ve analiz doğrulanmıştır. Kümeleme analizi ile veri seti yaşam tarzı metriklerine göre 2 ana profile ayrılmıştır.

## 🚀 Kullanım
Projedeki analizleri incelemek için ilgili klasörlerdeki script dosyalarını kullanabilir veya tüm yöntemlerin karşılaştırmalı sonuçları için doğrudan **`Analiz_Sonuc_Raporu.pdf`** dosyasını okuyabilirsiniz.
