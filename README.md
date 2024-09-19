# Mobil Ödeme Uygulamaları Yorum Analizi Projesi

Projenin Amacı:
Bu proje, Google Pay, Paytm ve PhonePe uygulamalarına ait kullanıcı yorumlarını analiz etmek amacıyla geliştirilmiştir. Veri setinde kullanıcıların puanları ve yorum içerikleri bulunmaktadır. Proje, kullanıcı deneyimini etkileyen faktörleri ve genel puan dağılımını incelemeyi amaçlamaktadır.

Veri Seti
Kullanılan veri seti, üç farklı mobil ödeme uygulamasından alınan yorumları içermektedir. Aşağıda sütun isimleri ve açıklamaları yer almaktadır:

userName: Kullanıcının adı
content: Kullanıcının yazdığı yorum
score: Kullanıcının verdiği puan
thumbsUpCount: Kullanıcı yorumuna verilen beğeni sayısı
score_class: Puanların medyana göre sınıflandırılması (0 ve 1)
Değişkenler
Bağımlı değişken (y) "score_class" sütunu olarak belirlenmiş, bağımsız değişkenler (X) ise "score" ve "thumbsUpCount" sütunları olarak tanımlanmıştır. Sınıflandırma algoritmaları kullanılarak bağımlı değişkenin tahmin edilmesi amaçlanmıştır. Kullanılan sınıflandırma algoritmaları:

Naive Bayes
Destek Vektör Makineleri (SVM)
Karar Ağaçları
Random Forest
Model Seçimi
Veri setindeki sınıf dengesizliği nedeniyle SMOTE (Synthetic Minority Over-sampling Technique) kullanılmaya çalışılmıştır. Ancak eğitim setinde yalnızca bir sınıf bulunduğu için bu adım gerçekleştirilememiştir. Sonuç olarak, her model için tahmin doğruluğu ve değerlendirme metrikleri hesaplanmıştır.

Değerlendirme Sürecinde Kullanılan Metrikler:

Doğruluk (Accuracy)
Karışıklık Matrisi (Confusion Matrix)
Sınıflandırma Raporu (Classification Report)
Görselleştirmeler
Proje kapsamında verilerin keşfi için çeşitli görselleştirmeler yapılmıştır:

Puan dağılımı histogramı
Korelasyon matrisinin heatmap'i
