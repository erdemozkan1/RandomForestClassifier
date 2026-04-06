# 📝 Adult Census Income Prediction with Random Forest
Bu proje, bireylerin demografik bilgilerini kullanarak yıllık gelirlerinin 50.000$ üzerinde olup olmadığını tahmin etmeyi amaçlayan bir makine öğrenmesi çalışmasıdır. Veri seti üzerinde veri temizleme, eksik değer doldurma ve sınıflandırma analizi uygulanmıştır.

🚀 Başarı Skoru (Performance)
Model, test verisi üzerinde yüksek bir doğruluk oranı yakalamıştır:

Accuracy: %86.6

### **Model**: *RandomForestClassifier*

### **Sınıflandırma Raporu (Classification Report)**
Plaintext
              precision    recall  f1-score   support
       <=50K       0.89      0.94      0.91      7444
        >50K       0.76      0.63      0.69      2325
🛠️ Kullanılan Teknolojiler
### Python 3.x

### Pandas & NumPy: Veri manipülasyonu ve analizi.

### Scikit-Learn: Makine öğrenmesi modeli ve ön işleme (preprocessing).

### Matplotlib & Seaborn: Veri görselleştirme.

🔍 Uygulanan Adımlar
Eksik Veri Yönetimi: workclass, occupation ve native_country sütunlarındaki eksik değerler mod (en sık geçen değer) ile dolduruldu.

Veri Temizleme: Kategorik verilerdeki gereksiz boşluklar (strip) temizlendi.

Encoding: Kategorik değişkenler modelin işleyebileceği sayısal formata dönüştürüldü.

Model Eğitimi: RandomForestClassifier algoritması kullanılarak eğitim gerçekleştirildi.

Hiperparametre Optimizasyonu: GridSearchCV ve n_jobs=-1 kullanılarak en iyi parametreler araştırıldı.

📈 Gelecek Çalışmalar
Sınıf Dengesizliği (Class Imbalance): Geliri >50K olan grubun yakalanma oranını (Recall) artırmak için SMOTE veya class_weight='balanced' teknikleri derinleştirilecek.

Model Karşılaştırma: XGBoost ve LightGBM gibi algoritmalar ile skorun %90 üzerine taşınması hedefleniyor.
## Dökümantasyon
https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
