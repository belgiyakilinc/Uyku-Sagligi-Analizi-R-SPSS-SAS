# Uyku Sağlığı ve Yaşam Tarzı: Çok Değişkenli İstatistiksel Analiz (R, SPSS, SAS)

[cite_start]Bu proje, "Sleep Health and Lifestyle Dataset" kullanılarak bireylerin uyku düzenleri ve yaşam tarzı alışkanlıkları arasındaki karmaşık ilişkileri inceleyen kapsamlı bir istatistiksel analiz çalışmasıdır[cite: 4, 13]. [cite_start]Çalışma kapsamında R, SPSS ve SAS yazılımları entegre bir şekilde kullanılmış ve çok değişkenli istatistiksel yöntemler uygulanmıştır.

## 📊 Veri Seti Hakkında
[cite_start]Veri seti, 374 bireye ait uyku süresi, uyku kalitesi, fiziksel aktivite seviyesi, stres düzeyi, kalp atış hızı, günlük adım sayısı ve uyku bozukluğu durumu (Yok, İnsomnia, Uyku Apnesi) gibi 13 farklı değişkeni içermektedir[cite: 13, 14, 28]. 

## 📁 Proje Dosya Yapısı
Depo içerisindeki analizler yöntemlerine göre aşağıdaki klasörlere ayrılmıştır:

* [cite_start]`Veri_Analizi/`: Değişkenlerin temel betimsel istatistikleri, çarpıklık/basıklık incelemeleri ve normallik testleri[cite: 34, 36, 131].
* [cite_start]`manova_analizi/`: Uyku bozukluğu türlerinin, uyku süresi ve kalitesi üzerindeki ortak etkisini inceleyen Çok Değişkenli Varyans Analizi kodları ve grafikleri[cite: 196, 197].
* [cite_start]`faktor_analizi/`: Veri setindeki gizli yapıyı ortaya çıkarmak için yapılan Temel Bileşenler ve Faktör Analizi uygulamaları[cite: 410, 436].
* [cite_start]`diskriminant_analizi/`: Bireylerin yaş, aktivite, uyku süresi ve kalitesine dayanarak hangi uyku bozukluğu grubuna ait olduklarını tahmin eden sınıflandırma modeli[cite: 466, 500].
* [cite_start]`logistik_regresyon_analizi/`: Uyku bozukluğu (Apne/İnsomnia) risk faktörlerini (yaş, stres, kalp atış hızı vb.) belirlemek için kurulan çok terimli lojistik regresyon modeli[cite: 561, 612].
* [cite_start]`kümeleme_analizi/`: Bireyleri sağlık ve yaşam tarzı benzerliklerine göre gruplara ayıran hiyerarşik ve k-ortalamalar (k-means) kümeleme analizi algoritmaları[cite: 643, 646].
* [cite_start]`Analiz_Sonuc_Raporu.pdf`: Tüm analiz çıktılarının, varsayım kontrollerinin ve istatistiksel yorumların bulunduğu detaylı final raporu[cite: 5].

## 📈 Temel Bulgular
Yapılan analizler sonucunda elde edilen başlıca istatistiksel bulgular şunlardır:

* [cite_start]**MANOVA:** Uyku bozukluğu (Özellikle Uyku Apnesi), bireylerin uyku süresi ve kalitesini istatistiksel olarak anlamlı düzeyde düşürmektedir ($p < 0.001$)[cite: 343, 348, 391, 406]. [cite_start]Ayrıca uyku apnesi yaş ile pozitif bir korelasyon göstermektedir[cite: 372].
* [cite_start]**Lojistik Regresyon:** Uyku kalitesindeki düşüş, stres seviyesindeki artış ve yaşın ilerlemesi, uyku apnesi ve insomnia riskini anlamlı şekilde artırmaktadır[cite: 621, 623, 624, 636, 638, 639]. [cite_start]Modelin genel sınıflandırma başarısı oldukça yüksektir (Örn: Uyku problemi olmayanları %93,2 oranında doğru tahmin etmiştir)[cite: 609].
* [cite_start]**Diskriminant Analizi:** Kurulan diskriminant fonksiyonları ile hastaların uyku bozukluğu grupları çapraz doğrulama (cross-validation) sonucunda %83,2 doğruluk oranıyla sınıflandırılmıştır[cite: 557].
* [cite_start]**Faktör ve Kümeleme Analizleri:** Faktör analizi öncesi KMO değeri 0.783 olarak bulunmuş ve analiz doğrulanmıştır[cite: 424]. [cite_start]Kümeleme analizi ile veri seti yaşam tarzı metriklerine göre 2 ana profile ayrılmıştır[cite: 646].

## 🚀 Kullanım
[cite_start]Projedeki analizleri incelemek için ilgili klasörlerdeki script dosyalarını kullanabilir veya tüm yöntemlerin karşılaştırmalı sonuçları için doğrudan **`Analiz_Sonuc_Raporu.pdf`** dosyasını okuyabilirsiniz[cite: 5].
