# BİL216 - Emo-Challenge 2026 (Grup 9)
**Ses İşareti Analizi ve Duygu Sınıflandırma Projesi**

Bu depo, insan sesinden duygu tespiti yapan makine öğrenmesi modellerimizin kaynak kodlarını içermektedir. Proje kapsamında kısıtlı ses verileri çoğaltılmış (Data Augmentation), frekans öznitelikleri (MFCC, Mel-Spectrogram) çıkarılmış ve çeşitli algoritmalarla test edilmiştir.

### 📁 Dosya Yapısı ve Kodlar
* `faz1_model.py`: Başlangıç seviyesi veri analizi ve ilk model denemeleri.
* `faz2_model.py`: Veri çoğaltma (White Noise, Pitch Shift) algoritmalarının uygulandığı ve SVM modelinin geliştirildiği script.
* `faz3_model.py`: **(🏆 ŞAMPİYON MODEL)** GridSearchCV ile hiperparametre optimizasyonu (C=200, gamma=0.01) yapılmış ve %85.51 accuracy oranına ulaşmış nihai kodumuz. Liderlik tablosu bu koda aittir.
* `faz3_cnn.py`: Mel-Spectrogram'lar üzerinden 2 boyutlu CNN mimarisi kurduğumuz derin öğrenme kodumuz. (Overfitting ve hata analizi detayları raporda mevcuttur).
* `faz3_gorseller.py`: Raporda kullanılan Confusion Matrix ve Spectrogram çizimlerini oluşturan istatistik scripti.
* `requirements.txt`: Projenin çalışması için gereken Python kütüphaneleri.

**Geliştiriciler:**
* Halil Nebi Kösebey
* Hüseyin Emir Abasız
* Ömer Hüseyin Ellidokuzoğlu
