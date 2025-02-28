

# Multi-Object Tracker

Bu proje, OpenCV kullanarak gerçek zamanlı nesne takibi gerçekleştiren bir uygulamadır. Kullanıcı, video akışında bir veya daha fazla nesne seçebilir ve bu nesneleri farklı takip algoritmalarıyla izleyebilir. Proje, OpenCV'nin `MultiTracker` fonksiyonunu ve farklı takip algoritmalarını (CSRT, KCF, MedianFlow, vb.) kullanarak nesne takibini yönetir.

## Özellikler

- Gerçek zamanlı nesne takibi
- Kullanıcı tarafından seçilen nesnelerin takibi
- Çeşitli OpenCV takip algoritmalarının desteği (CSRT, KCF, MedianFlow, vb.)
- Takip edilen nesneler için GUI üzerinden bilgi sağlama
- Kullanıcıya birden fazla nesne seçme ve takip algoritması seçme imkanı

## Kullanım

1. **Gerekli Kütüphanelerin Yüklenmesi:**

   Bu projeyi çalıştırmadan önce gerekli Python kütüphanelerini yüklemeniz gerekmektedir. Şu komutla yükleyebilirsiniz:

   ```bash
   pip install opencv-python numpy
Programı Çalıştırma:

Projeyi çalıştırmak için aşağıdaki komutu kullanabilirsiniz:

bash
Kopyala
python multi_object_tracker.py
Nesne Takibi Başlatma:

Video akışı başladıktan sonra, bir nesne seçmek için fare ile üzerine tıklayın ve seçim yapın.
Bir nesne seçtikten sonra, başka bir nesne seçmek için 's' tuşuna basarak başka bir ROI (Region of Interest) seçebilirsiniz.
Takip algoritması hakkında bilgi almak için ekranın sol üst kısmında "Tracker" ve "Success" bilgileri görünecektir.
Takip Algoritması Seçme:

Program, başlangıçta MedianFlow algoritmasını kullanacaktır.
Farklı bir algoritma seçmek isterseniz, kodda tracker_name değişkenini değiştirebilirsiniz.
Programdan Çıkma:

Takip işlemini sonlandırmak için 'q' tuşuna basabilirsiniz.
Takip Algoritmaları
Bu projede kullanılan takip algoritmaları şunlardır:

CSRT (Discriminative Correlation Filter with Channel and Spatial Reliability)
KCF (Kernelized Correlation Filters)
Boosting
MIL (Multiple Instance Learning)
TLD (Tracking-Learning-Detection)
MedianFlow
MOSSE
Kod Yapısı
multi_object_tracker.py: Nesne takibi yapan ana Python dosyası.


