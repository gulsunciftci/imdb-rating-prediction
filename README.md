# 🎬 IMDb Film Puanı Tahmini (Regresyon)

Bu proje, IMDb veri setinde yer alan filmlerin bazı özelliklerini (süre, bütçe, oy sayısı vb.) kullanarak, IMDb puanlarını tahmin etmek amacıyla bir **doğrusal regresyon modeli** (Linear Regression) geliştirir.

Makine öğrenmesine giriş seviyesi için uygun, anlaşılır ve uygulanabilir bir örnektir.

---

## 📦 Kullanılan Kütüphaneler

- Python 3.x  
- pandas  
- scikit-learn  
- matplotlib  
- seaborn  

---

## 🧠 Kullanılan Özellikler (Features)

| Özellik | Açıklama |
|---------|----------|
| `duration` | Filmin süresi (dakika) |
| `budget` | Film bütçesi |
| `gross` | Gişe hasılatı |
| `num_voted_users` | IMDb'de oy kullanan kullanıcı sayısı |
| `cast_total_facebook_likes` | Oyuncuların toplam Facebook beğenisi |

🎯 **Hedef Değişken:** `imdb_score`

---

## 🔧 Modelleme Adımları

1. Veriyi `movie_metadata.csv` dosyasından oku  
2. Eksik verileri temizle (`dropna()`)  
3. Giriş ve hedef değişkenleri ayır (`X`, `y`)  
4. Eğitim ve test setlerine böl (%80 eğitim, %20 test)  
5. Doğrusal regresyon modeli ile eğit  
6. Tahmin yap ve performansı ölç (`R²`, `RMSE`)  
7. Tahminleri grafiklerle analiz et

---

## 📈 Model Performansı

- **RMSE (Ortalama Karekök Hatası):** ~0.88  
- **R² Skoru (Açıklanan Varyans):** ~0.29 
(*Değerler kullanılan veri setine göre değişebilir.*)

---

## 📊 Görselleştirmeler

- Scatter plot: Gerçek vs Tahmin IMDb puanları  
- Histogram: Tahmin hatalarının dağılımı  
- Kırmızı çizgi: Mükemmel tahmini gösteren y=x çizgisi

---

## 🚀 Nasıl Çalıştırılır?

1. Gerekli kütüphaneleri kur:
```pip install pandas scikit-learn matplotlib seaborn```
2. Proje dosyalarını indir

3. Jupyter Notebook veya .py dosyasını çalıştır

4. movie_metadata.csv dosyasını proje klasörüne koy
