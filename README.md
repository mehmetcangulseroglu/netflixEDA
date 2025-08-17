# Netflix Veri Analizi Projesi

Bu proje, Netflix içeriklerine ilişkin bir veri setinin keşifsel veri analizini (EDA) içeren bir Jupyter Notebook çalışmasıdır. Analiz, veri setinin yapısını, eksik değerlerini ve temel istatistiklerini derinlemesine incelemektedir.

## 📊 Proje Hakkında

Netflix platformundaki film ve TV şovlarının çeşitli özelliklerini analiz ederek içerik dağılımları, trendler ve örüntüler hakkında bilgi edinmeyi amaçlayan bir veri bilimi projesidir.

## 🛠️ Kullanılan Kütüphaneler

- **numpy**: Sayısal işlemler ve matematiksel hesaplamalar için
- **pandas**: Veri işleme, manipülasyon ve analiz için
- **matplotlib.pyplot**: Temel veri görselleştirme için
- **seaborn**: Gelişmiş istatistiksel veri görselleştirme için

## 📁 Veri Seti

Proje `netflix_titles.csv` dosyasını kullanmaktadır. Bu veri seti aşağıdaki sütunları içerir:

| Sütun Adı | Açıklama |
|-----------|----------|
| `show_id` | İçerik kimliği |
| `type` | İçerik türü (Film veya TV Şovu) |
| `title` | İçerik başlığı |
| `director` | Yönetmen bilgisi |
| `cast` | Oyuncular |
| `country` | Üretim ülkesi |
| `date_added` | Netflix'e eklenme tarihi |
| `release_year` | Yayınlanma yılı |
| `rating` | İçerik derecelendirmesi |
| `duration` | Süre (dakika veya sezon sayısı) |
| `listed_in` | Kategoriler/Türler |
| `description` | İçerik açıklaması |

## 🔍 Analiz Adımları

### 1. Veri Yükleme ve İlk İnceleme
- Veri setinin pandas kütüphanesi ile yüklenmesi
- İlk 5 satırın görüntülenmesi
- Veri setinin boyutlarının kontrolü

### 2. Veri Kalitesi Değerlendirmesi
- Eksik değerlerin tespiti ve analizi
- Her sütundaki benzersiz değerlerin incelenmesi
- Veri türlerinin kontrolü

### 3. Veri Temizleme
- Eksik veriler içeren satırların kaldırılması
- Veri setinin optimize edilmesi

### 4. Görselleştirme ve Analiz
- **İçerik Türü Dağılımı**: Film ve TV şovu oranları
- **Derecelendirme Analizi**: Yaş sınırlaması kategorilerinin dağılımı
- **Trend Analizleri**: Yıllara göre içerik eklenme trendleri

## 📈 Temel Bulgular

- **Veri Seti Boyutu**: 8,807 satır ve 12 sütun
- **Temizlenmiş Veri**: 5,332 satır (eksik veriler çıkarıldıktan sonra)
- **En Yaygın İçerik Türü**: Film (Movie)
- **Popüler Derecelendirmeler**: TV-MA ve TV-14 kategorileri

## 🚀 Kurulum ve Çalıştırma

### Gereksinimler
```bash
pip install numpy pandas matplotlib seaborn jupyter
```

### Adım Adım Kullanım

1. **Gerekli kütüphaneleri içe aktarın:**
```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

2. **Veri setini yükleyin:**
```python
netflix = pd.read_csv("netflix_titles.csv")
```

3. **Jupyter Notebook'u başlatın:**
```bash
jupyter notebook
```

4. **Notebook dosyasını açın ve analiz adımlarını çalıştırın**

## 🤝 Katkıda Bulunma

Bu proje açık kaynaklıdır ve katkılara açıktır. Katkıda bulunmak için:

1. Bu repository'yi fork edin
2. Yeni bir branch oluşturun (`git checkout -b feature/yeni-ozellik`)
3. Değişikliklerinizi commit edin (`git commit -am 'Yeni özellik eklendi'`)
4. Branch'inizi push edin (`git push origin feature/yeni-ozellik`)
5. Pull Request oluşturun

## 📧 İletişim

Sorularınız veya önerileriniz için issue açabilir veya pull request gönderebilirsiniz.

---

⭐ Bu projeyi beğendiyseniz, yıldız vermeyi unutmayın!
