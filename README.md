# BİL216 - Emo-Challenge 2026 (Grup 9)
**Ses İşareti Analizi ve Duygu Sınıflandırma Projesi**

Bu depo, insan sesinden duygu tespiti yapan makine öğrenmesi modellerimizin kaynak kodlarını içermektedir. Proje kapsamında kısıtlı ses verileri çoğaltılmış (Data Augmentation), frekans öznitelikleri (MFCC, Mel-Spectrogram) çıkarılmış ve çeşitli algoritmalarla test edilmiştir.

### 📁 Dosya Yapısı ve Kodlar
* `faz-1.py`: Başlangıç seviyesi veri analizi ve ilk model denemeleri.
* `faz-2.py`: Veri çoğaltma (White Noise, Pitch Shift) algoritmalarının uygulandığı ve SVM modelinin geliştirildiği script.
* `faz3_model.py`: **(🏆 ŞAMPİYON MODEL)** GridSearchCV ile hiperparametre optimizasyonu (C=200, gamma=0.01) yapılmış ve %85.51 accuracy oranına ulaşmış nihai kodumuz. Liderlik tablosu bu koda aittir.
* `faz3_cnn.py`: Mel-Spectrogram'lar üzerinden 2 boyutlu CNN mimarisi kurduğumuz derin öğrenme kodumuz. (Overfitting ve hata analizi detayları raporda mevcuttur).
* `faz3_gorseller.py`: Raporda kullanılan Confusion Matrix ve Spectrogram çizimlerini oluşturan istatistik scripti.

**Geliştiriciler:**
* Halil Nebi Kösebey
* Hüseyin Emir Abasız
* Ömer Hüseyin Ellidokuzoğlu

# ─────────────────────────────────────────────────────────────────
# DSP Projesi – Python Bağımlılıkları
# Kurulum: pip install -r requirements.txt
# Python 3.10+ gereklidir
# ─────────────────────────────────────────────────────────────────

# Ses işleme
librosa>=0.10.0
soundfile>=0.12.0

# Sayısal hesaplama
numpy>=1.24.0
scipy>=1.11.0

# Veri yönetimi
pandas>=2.0.0
openpyxl>=3.1.0        # Excel (.xlsx) okuma/yazma için

# Görselleştirme
matplotlib>=3.7.0
seaborn>=0.12.0

# Web arayüzü
streamlit>=1.30.0

# Makine öğrenmesi (sadece confusion matrix / accuracy için)
scikit-learn>=1.3.0
