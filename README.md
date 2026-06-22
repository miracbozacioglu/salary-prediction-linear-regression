<div align="center">

# 💼 Basit Doğrusal Regresyon ile Maaş Tahmini

**Deneyim yılına göre maaş tahmini yapan, uçtan uca bir makine öğrenmesi projesi**

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)
![R²](https://img.shields.io/badge/R²_Skoru-0.9882-success)

</div>

---

Bu proje, **basit doğrusal regresyon (simple linear regression)** algoritmasını kullanarak bir çalışanın **deneyim yılına** göre **maaşını** tahmin eder. Denetimli öğrenmenin (supervised learning) temellerini ve uçtan uca bir model geliştirme akışını adım adım göstermek için hazırlanmıştır.

## 📋 İçindekiler

- [🎯 Proje Hakkında](#-proje-hakkında)
- [📊 Veri Seti](#-veri-seti)
- [🛠️ Kullanılan Teknolojiler](#️-kullanılan-teknolojiler)
- [⚙️ Kurulum](#️-kurulum)
- [🚀 Kullanım](#-kullanım)
- [📈 Model ve Sonuçlar](#-model-ve-sonuçlar)
- [📁 Proje Yapısı](#-proje-yapısı)
- [📄 Lisans](#-lisans)

## 🎯 Proje Hakkında

Proje, bir makine öğrenmesi modelinin yaşam döngüsünü altı temel adımda ele alır:

| # | Adım | Açıklama |
|---|------|----------|
| 1 | **Veri Yükleme ve İnceleme** | Veri setinin okunması ve istatistiksel özetinin çıkarılması |
| 2 | **Görselleştirme** | Deneyim–maaş ilişkisinin saçılım grafiği (scatter plot) ile incelenmesi |
| 3 | **Veri Hazırlama** | Bağımsız (X) ve bağımlı (y) değişkenlerin ayrılması, eğitim/test bölünmesi |
| 4 | **Model Eğitimi** | `LinearRegression` modelinin eğitim verisi üzerinde eğitilmesi |
| 5 | **Değerlendirme** | Modelin R² skoru ve MSE metrikleriyle ölçülmesi |
| 6 | **Tahmin** | Eğitilen model ile yeni bir gözlem için maaş tahmini |

## 📊 Veri Seti

`Salary_Data.csv` dosyası **30 gözlemden** oluşur ve iki sütun içerir:

| Sütun | Açıklama |
|-------------------|------------------------------------|
| `YearsExperience` | Çalışanın yıl cinsinden deneyimi |
| `Salary` | Çalışanın maaşı |

## 🛠️ Kullanılan Teknolojiler

| Teknoloji | Kullanım Amacı |
|------------------|------------------------------|
| **Python 3** | Programlama dili |
| **NumPy** | Sayısal işlemler |
| **Pandas** | Veri yükleme ve manipülasyonu |
| **Matplotlib** | Veri görselleştirme |
| **scikit-learn** | Model eğitimi ve değerlendirme |
| **Jupyter** | Geliştirme ortamı |

## ⚙️ Kurulum

**1.** Depoyu klonlayın:

```bash
git clone https://github.com/<kullanici-adi>/simple_linear_regression.git
cd simple_linear_regression
```

**2.** (Önerilen) Bir sanal ortam oluşturun ve etkinleştirin:

```bash
python -m venv venv

# Windows
venv\Scripts\activate

# macOS / Linux
source venv/bin/activate
```

**3.** Gerekli kütüphaneleri yükleyin:

```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

## 🚀 Kullanım

Jupyter Notebook'u başlatın ve not defterini açın:

```bash
jupyter notebook simple_linear.ipynb
```

Hücreleri sırayla çalıştırarak veri analizinden model tahminine kadar tüm akışı adım adım izleyebilirsiniz.

## 📈 Model ve Sonuçlar

Model, verinin **%80'i ile eğitilmiş**, **%20'si ile test edilmiştir**. Test verisi üzerinde elde edilen sonuçlar:

| Metrik | Değer |
|----------------------------------|----------------|
| **R² Skoru** (R-Squared) | `0.9882` |
| **Hata Kareler Ortalaması** (MSE) | `12.823.412,30` |

> 📌 **0.9882** R² skoru, modelin maaştaki değişkenliğin yaklaşık **%98'ini** açıkladığını ve deneyim ile maaş arasında oldukça güçlü bir doğrusal ilişki olduğunu gösterir.

🔮 **Örnek tahmin:** 5.5 yıllık deneyime sahip bir kişi için tahmin edilen maaş ≈ **77.999,26**

## 📁 Proje Yapısı

```
simple_linear_regression/
├── 📄 Salary_Data.csv        # Veri seti
├── 📓 simple_linear.ipynb    # Analiz ve model not defteri
└── 📘 README.md              # Proje dokümantasyonu
```

## 📄 Lisans

Bu proje açık kaynaklıdır ve eğitim amaçlı serbestçe kullanılabilir.

<div align="center">

⭐ Beğendiyseniz projeye yıldız vermeyi unutmayın!

</div>
