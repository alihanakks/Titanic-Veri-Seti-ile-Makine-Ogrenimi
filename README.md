# 🚢 Titanic Hayatta Kalma Tahmini

Bu proje, Titanic verisi üzerinde makine öğrenmesi algoritmaları ile hayatta kalma durumunu tahmin etmeyi amaçlamaktadır.

## 📌 Proje Özeti

Bu çalışma aşağıdaki adımları içermektedir:

- Veri Temizleme ve Hazırlama
- Özellik Mühendisliği
- Modelleme: Random Forest & XGBoost
- Hiperparametre Ayarı (GridSearchCV)
- Model Performans Değerlendirmesi

## 📊 Kullanılan Veri

Veri seti, [Kaggle Titanic yarışması](https://www.kaggle.com/c/titanic) kapsamında sağlanan klasik Titanic veri setidir.

## ⚙️ Kullanılan Modeller

- Random Forest Sınıflandırıcı
- XGBoost Sınıflandırıcı
- Değerlendirme metrikleri: Doğruluk (Accuracy), Precision, Recall, F1-Score

## 🎯 Sonuçlar

| Model | Doğruluk | Sınıf 1 Recall | Sınıf 1 F1-Score |
|-------|----------|----------------|------------------|
| Random Forest (varsayılan) | 0.79 | 0.66 | 0.71 |
| XGBoost (varsayılan) | 0.78 | 0.65 | 0.69 |
| **Random Forest (optimize)** | **0.80** | **0.68** | **0.72** |
| XGBoost (optimize) | 0.78 | 0.60 | 0.67 |

**Random Forest** algoritması, optimize edilmiş haliyle en başarılı sonuçları vermiştir.

## 🔧 Gereksinimler

Aşağıdaki kütüphanelerin kurulu olması gerekir:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
