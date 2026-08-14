Özet 

Bu projede, öğrencilerin bir yapay zekâ asistanını tekrar kullanıp kullanmayacağını tahmin etmek amacıyla uçtan uca bir makine öğrenmesi süreci uygulanmıştır. Çalışma kapsamında veri inceleme, veri ön işleme, öznitelik mühendisliği, öznitelik seçimi, model eğitimi, model karşılaştırması, hiperparametre optimizasyonu, model değerlendirme ve açıklanabilirlik analizi gerçekleştirilmiştir.

Veri Seti

Veri seti, öğrencilerin yapay zekâ asistanı kullanımına ait oturum bilgilerini içermektedir. Kullanılan başlıca değişkenler:

Oturum süresi (SessionLengthMin)
Prompt sayısı (TotalPrompts)
Yapay zekâ yardım seviyesi (AI_AssistanceLevel)
Memnuniyet puanı (SatisfactionRating)
Öğrenci seviyesi
Bölüm bilgisi
Görev türü
Oturum sonucu
Tekrar kullanım bilgisi (UsedAgain)

Hedef değişken: UsedAgain (True / False)

Kullanılan Modeller
Logistic Regression
K-Nearest Neighbors (KNN)
Decision Tree
En İyi Model Sonuçları

En başarılı model Logistic Regression olmuştur.

Validation Accuracy: %75.6
Test Accuracy: %74.25
Precision: %79.46
Recall: %85.70
F1-score: %82.47


Önemli Bulgular
Kodlama görevleri tekrar kullanım olasılığını artırmaktadır.
Oturumu “Confused” veya “Gave Up” sonucu ile tamamlayan kullanıcıların tekrar kullanım olasılığı belirgin biçimde düşmektedir.
Üretilen 'PromptDensity' ve 'EngagementScore' öznitelikleri kullanıcı davranışını daha iyi temsil etmiştir.


Proje Dosyaları
student_ai_reuse_prediction.ipynb → Ana çalışma dosyası
ai_assistant_usage_student_life.csv → Veri seti
requirements.txt → Gerekli Python kütüphaneleri
README.md → Proje açıklaması


Çalıştırma Adımları

Gerekli kütüphaneleri yüklemek için:

pip install -r requirements.txt

Ardından notebook dosyasını açıp tüm hücreleri sırayla çalıştırınız.

Sonuç

Bu proje, öğrencilerin yapay zekâ asistanını tekrar kullanma davranışını tahmin etmek için eksiksiz bir makine öğrenmesi iş akışı sunmaktadır. Seçilen Logistic Regression modeli daha önce görmediği veriler üzerinde tutarlı performans göstermiş ve kullanıcı davranışına ilişkin yorumlanabilir çıktılar üretmiştir.
