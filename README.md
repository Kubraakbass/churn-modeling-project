Proje Hakkında

Bu proje, bankacılık sektöründe müşteri terk etme (churn) davranışını tahmin etmek için geliştirilmiştir. Amaç, hangi müşterilerin bankadan ayrılma ihtimali olduğunu önceden tespit ederek müşteri kaybını azaltmaktır.

Makine öğrenmesi sınıflandırma algoritmaları kullanılarak müşteri davranışları analiz edilmiştir.

 Veri Seti

Kullanılan veri seti: Churn_Modelling.csv

Veri seti aşağıdaki müşteri bilgilerini içerir:

Credit Score (Kredi skoru)
Geography (Ülke)
Gender (Cinsiyet)
Age (Yaş)
Tenure (Müşteri süresi)
Balance (Bakiye)
NumOfProducts (Ürün sayısı)
HasCrCard (Kredi kartı var mı)
IsActiveMember (Aktif üye durumu)
EstimatedSalary (Tahmini maaş)
Target: Exited (0 = Ayrılmadı, 1 = Ayrıldı)
 Proje Aşamaları
1. Veri Ön İşleme
Kategorik değişkenlerin dönüştürülmesi (Encoding)
Özellik ölçeklendirme (Feature Scaling)
Eksik veri kontrolü
2. Keşifsel Veri Analizi (EDA)
Veri dağılımlarının incelenmesi
Korelasyon analizi
Churn oranlarının görselleştirilmesi
3. Modelleme
Logistic Regression / Random Forest Classifier kullanıldı
Veri train-test olarak ayrıldı
4. Model Değerlendirme
Accuracy (Doğruluk)
Precision (Kesinlik)
Recall (Duyarlılık)
F1-score
Confusion Matrix
 Model Sonuçları
 Sınıf 0 (Ayrılmayan Müşteriler)
Precision: 0.86
Recall: 0.98
F1-score: 0.91
Sınıf 1 (Ayrılan Müşteriler)
Precision: 0.82
Recall: 0.36
F1-score: 0.50
   Sonuç Değerlendirmesi

Model genel olarak yüksek doğruluk (≈ %85) elde etmiştir. Ancak veri seti dengesiz olduğu için accuracy tek başına yeterli bir metrik değildir.

Asıl önemli olan churn (Class 1) tespitidir. Bu sınıfta recall değerinin düşük olması, ayrılan müşterilerin büyük bir kısmının model tarafından kaçırıldığını göstermektedir.

Bu durum, gerçek hayatta müşteri kaybı açısından kritik bir problemdir.

🚀 Geliştirme Önerileri

Model performansını artırmak için:

SMOTE (veri dengeleme) uygulanabilir
class_weight parametresi kullanılabilir
Threshold tuning yapılabilir
Daha güçlü modeller (XGBoost, LightGBM) denenebilir
Hiperparametre optimizasyonu yapılabilir
 Kullanılan Teknolojiler
Python 
Pandas & NumPy
Scikit-learn
Matplotlib & Seaborn
Jupyter Notebook
 İş Etkisi

Bu model bankalar için:

Müşteri kaybını azaltma
Riskli müşterileri önceden tespit etme
Pazarlama stratejilerini geliştirme
Gelir artırma fırsatı sağlar
 Proje Sahibi

Veri bilimi ve makine öğrenmesi alanında çalışan bir öğrenci tarafından geliştirilmiştir.

 Not

Bu proje, sınıflandırma problemleri ve veri analizi konusunda temel–orta seviye bir makine öğrenmesi çalışmasıdır.
