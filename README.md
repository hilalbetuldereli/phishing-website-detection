
---

# 🛡️ Phishing Website Detection

**Makine Öğrenmesi Tabanlı Phishing Web Sitesi Tespiti**

Bu proje, phishing (oltalama) web sitelerinin **makine öğrenmesi yöntemleri** kullanılarak tespit edilmesini amaçlamaktadır. Çalışmada URL ve içerik tabanlı özellikler kullanılarak **Logistic Regression** ve **Random Forest** modelleri eğitilmiş, performansları karşılaştırılmış ve en başarılı model **Gradio tabanlı bir web arayüzü** ile sunulmuştur.

📌 Bu çalışma, **Veri Bilimine Giriş dersi** kapsamında hazırlanmıştır.

---

## 📂 Proje İçeriği

```
phishing-website-detection/
│
├── phishing_detection.ipynb
├── README.md
└── veribiliminegirisrapor.docx

```

📌 Tüm veri analizi, model eğitimi, değerlendirme ve Gradio uygulaması **tek bir Jupyter Notebook** içerisinde yer almaktadır.

---

## 🎯 Proje Amaçları

* Phishing ve güvenli web sitelerini ayırt edebilen bir sınıflandırma modeli geliştirmek
* Logistic Regression ve Random Forest algoritmalarını karşılaştırmak
* Model performanslarını accuracy, precision, recall ve F1-score metrikleri ile değerlendirmek
* Gradio kullanarak kullanıcı dostu bir tahmin arayüzü oluşturmak

---

## 📊 Veri Seti

* **Kaynak:** Kaggle – *Phishing Dataset for Machine Learning*
* **Toplam örnek:** 10.000
* **Sınıf dağılımı:** Dengeli (Phishing / Güvenli)
* **Özellik sayısı:** 48
* **Eksik veri:** Yok

Veri setinde URL yapısı, alan adı bilgileri ve form güvenliği gibi phishing tespitinde kritik öneme sahip öznitelikler bulunmaktadır.

---

## ⚙️ Kullanılan Teknolojiler

* **Programlama Dili:** Python
* **Notebook Ortamı:** Jupyter Notebook / Google Colab
* **Veri Analizi:** Pandas, NumPy
* **Görselleştirme:** Matplotlib, Seaborn
* **Makine Öğrenmesi:** Scikit-learn
* **Model Kaydetme:** Joblib
* **Web Arayüzü:** Gradio

---

## 🤖 Kullanılan Modeller

### 🔹 Logistic Regression

* Baseline model olarak kullanılmıştır
* Doğrusal ve yorumlanabilir yapı sunar

### 🔹 Random Forest

* Ana sınıflandırma modeli
* Karmaşık ilişkileri öğrenebilme yeteneğine sahiptir
* Logistic Regression’a kıyasla daha yüksek performans elde edilmiştir

---

## 📈 Model Performansı

| Model               | Accuracy | Precision | Recall   | F1-Score |
| ------------------- | -------- | --------- | -------- | -------- |
| Logistic Regression | 0.95     | 0.95      | 0.95     | 0.95     |
| **Random Forest**   | **0.98** | **0.99**  | **0.98** | **0.98** |

📌 Phishing tespitinde **recall** metriği kritik olduğu için Random Forest modeli tercih edilmiştir.

---

## 🌐 Gradio Web Arayüzü

Notebook içerisinde, eğitilen model **Gradio** kullanılarak web tabanlı bir arayüze dönüştürülmüştür.

**Arayüz Özellikleri:**

* Slider, dropdown ve number girişleri
* Gerçek zamanlı tahmin
* Olasılık değeri ile birlikte sonuç gösterimi

Örnek çıktı:

* 🎣 *Phishing (0.51)*
* ✅ *Güvenli (0.49)*


---

## ▶️ Çalıştırma

Bu proje **tek bir Jupyter Notebook** üzerinden çalışmaktadır.

### Google Colab ile

1. Repository’yi klonla veya `.ipynb` dosyasını indir
2. Google Colab’da aç
3. Hücreleri sırasıyla çalıştır
4. Gradio arayüzü otomatik olarak başlatılır

### Lokal Jupyter ile

```bash
pip install pandas numpy scikit-learn matplotlib seaborn gradio joblib
jupyter notebook phishing_detection.ipynb
```

---

## 📄 Rapor

Detaylı proje raporu, akademik formatta hazırlanmıştır ve projede kullanılan tüm yöntemleri kapsamaktadır.



---

## 📚 Kaynaklar

* Kaggle – Phishing Dataset for Machine Learning
* Scikit-learn Documentation
* Gradio Documentation

---

