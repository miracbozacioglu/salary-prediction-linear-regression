# Basit Doğrusal Regresyon ile Maaş Tahmini

Bu proje, **basit doğrusal regresyon (simple linear regression)** algoritması kullanarak bir çalışanın **deneyim yılına** göre **maaşını** tahmin eden bir makine öğrenmesi uygulamasıdır. Proje, denetimli öğrenmenin (supervised learning) temellerini ve uçtan uca bir model geliştirme akışını göstermek amacıyla hazırlanmıştır.

## 📋 İçindekiler

- [Proje Hakkında](#-proje-hakkında)
- [Veri Seti](#-veri-seti)
- [Kullanılan Teknolojiler](#-kullanılan-teknolojiler)
- [Kurulum](#-kurulum)
- [Kullanım](#-kullanım)
- [Model ve Sonuçlar](#-model-ve-sonuçlar)
- [Proje Yapısı](#-proje-yapısı)
- [Lisans](#-lisans)

## 🎯 Proje Hakkında

Proje aşağıdaki adımlardan oluşur:

1. **Veri Yükleme ve İnceleme** – Veri setinin okunması ve istatistiksel özetinin çıkarılması.
2. **Görselleştirme** – Deneyim ile maaş arasındaki ilişkinin saçılım grafiği (scatter plot) ile incelenmesi.
3. **Veri Hazırlama** – Bağımsız değişken (X) ve bağımlı değişkenin (y) ayrılması, eğitim/test olarak bölünmesi.
4. **Model Eğitimi** – `LinearRegression` modelinin eğitim verisi üzerinde eğitilmesi.
5. **Değerlendirme** – Modelin R² skoru ve MSE (Hata Kareler Ortalaması) metrikleriyle değerlendirilmesi.
6. **Tahmin** – Eğitilen model ile yeni bir gözlem için maaş tahmini yapılması.

## 📊 Veri Seti

`Salary_Data.csv` dosyası 30 gözlemden oluşur ve iki sütun içerir:

| Sütun | Açıklama |
|-------------------|------------------------------------|
| `YearsExperience` | Çalışanın yıl cinsinden deneyimi |
| `Salary` | Çalışanın maaşı |

## 🛠️ Kullanılan Teknolojiler

- **Python 3**
- **NumPy** – Sayısal işlemler
- **Pandas** – Veri yükleme ve manipülasyonu
- **Matplotlib** – Veri görselleştirme
- **scikit-learn** – Model eğitimi ve değerlendirme
- **Jupyter Notebook** – Geliştirme ortamı

## ⚙️ Kurulum

1. Depoyu klonlayın:

   ```bash
   git clone https://github.com/<kullanici-adi>/simple_linear_regression.git
   cd simple_linear_regression
   ```

2. (Önerilen) Bir sanal ortam oluşturun ve etkinleştirin:

   ```bash
   python -m venv venv
   # Windows
   venv\Scripts\activate
   # macOS / Linux
   source venv/bin/activate
   ```

3. Gerekli kütüphaneleri yükleyin:

   ```bash
   pip install numpy pandas matplotlib scikit-learn jupyter
   ```

## 🚀 Kullanım

Jupyter Notebook'u başlatın ve dosyayı açın:

```bash
jupyter notebook simple_linear.ipynb
```

Hücreleri sırayla çalıştırarak veri analizinden model tahminine kadar tüm akışı izleyebilirsiniz.

## 📈 Model ve Sonuçlar

Model, verinin **%80'i ile eğitilmiş**, **%20'si ile test edilmiştir**. Test verisi üzerinde elde edilen sonuçlar:

| Metrik | Değer |
|----------------------------|----------------|
| R² Skoru (R-Squared) | 0.9882 |
| Hata Kareler Ortalaması (MSE) | 12.823.412,30 |

**0.9882** R² skoru, modelin maaştaki değişkenliğin yaklaşık **%98'ini** açıkladığını ve deneyim ile maaş arasında oldukça güçlü bir doğrusal ilişki olduğunu gösterir.

> Örnek tahmin: 5.5 yıllık deneyime sahip bir kişi için tahmin edilen maaş ≈ **77.999,26**

## 📁 Proje Yapısı

```
simple_linear_regression/
├── Salary_Data.csv        # Veri seti
├── simple_linear.ipynb    # Analiz ve model not defteri
└── README.md              # Proje dokümantasyonu
```

## 📄 Lisans

Bu proje eğitim amaçlıdır ve [MIT Lisansı](LICENSE) ile lisanslanmıştır.
