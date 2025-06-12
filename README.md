# Air France Yorumlarında Duygu Analizi (NLP Projesi)

Bu proje, **Air France** havayolu şirketine ait müşteri yorumlarını kullanarak metin madenciliği ve duygu analizi gerçekleştirmektedir. Yorum metinleri temizlenmiş, TF-IDF yöntemi ile sayısal forma dönüştürülmüş ve çeşitli makine öğrenmesi algoritmalarıyla sınıflandırma yapılmıştır.

## Proje Hedefi
Air France müşteri yorumlarını **pozitif**, **negatif** veya **nötr** olarak sınıflandırmak ve bu sayede havayolu firmasının müşteri memnuniyeti hakkında çıkarımlar yapmak.

## Kullanılan Veri Seti
- **Kaynak:** [Kaggle - Air France Tripadvisor Reviews Dataset](https://www.kaggle.com/datasets/saharnazyaghoobpoor/air-france-reviews-dataset)
- **Boyut:** Yaklaşık 7.000 yorum
- **Sütunlar:** `rating`, `title`, `text`, `publishedDate`

## 🛠️ Kullanılan Teknolojiler
- **Programlama Dili:** Python (Jupyter Notebook)
- **Kütüphaneler:**
  - pandas  
  - scikit-learn  
  - matplotlib  
  - seaborn  
  - wordcloud

## Yöntemler

### 📝 Metin Ön İşleme
- Küçük harfe çevirme  
- Noktalama kaldırma  
- Stop word temizliği  
- Metin birleştirme (`title` + `text`)

### Özellik Çıkarımı
- **TF-IDF vektörleştirme** (maks. 1000 kelime)

### Sınıflandırma Algoritmaları
- Naive Bayes  
- Logistic Regression  
- Random Forest

### Değerlendirme Metrikleri
- Accuracy (Doğruluk)  
- Precision  
- Recall  
- F1-score

## Görselleştirmeler
### Confusion Matrix
<img src="Confusion Matrix.png" width="300"/>

### Puan Dağılımı
<img src="Puan Dağılımı.png" width="300"/>

### Sentiment Dağılımı
<img src="Sentiment Dağılımı.png" width="300"/>

### WordCloud
<img src="WordCloud.png" width="300"/>

### Yorum Uzunluğu Dağılımı
<img src="Yorum Uzunluğu Dağılımı.png" width="300"/>

## Sonuçlar
- **Logistic Regression** modeli ikili sınıflandırmada en yüksek başarıyı göstermiştir.
- **Random Forest**, üç sınıflı analizde daha dengeli sonuçlar vermiştir.
- **Nadir kelimeler**, IDF değerlerine göre belirlenmiş ve analiz edilmiştir.

## Ekler
- `airfrance_sentiment_analysis.ipynb` → Ana çalışma dosyası  
- `rapor.docx` → Proje raporu  
- `grafikler/` → WordCloud ve confusion matrix görselleri

## Katkı
Bu proje, **Python ile Veri Bilimi** dersi kapsamında; metin madenciliği, veri ön işleme ve temel sınıflandırma tekniklerini uygulamalı olarak göstermek amacıyla hazırlanmıştır.
