# Brain_Tumor_Detection

## Akbank Derin Öğrenmeye Giriş Bootcampi
Akbank Gençlik Akademisi ve Global AI Hub iş birliğiyle gerçekleştirilen bir aylık Derin Öğrenmeye Giriş Bootcampi kapsamında hazırlanan bitirme projesidir. Projenin amacı, beyin MR görüntüleri üzerinden beyin tümörlerini otomatik olarak sınıflandırabilen bir derin öğrenme modeli geliştirmektir. Başta değerli leadimiz Göker Güner olmak üzere diğer lead ve mentörlerimize bu yolculukta bizlere eşlik ederek bilgi birikimlerini bizimle paylaştıkları için teşekkürlerimi sunuyorum.

## Giriş
Bu proje, beyin tümörü tespiti için derin öğrenme tabanlı bir görüntü sınıflandırma çalışmasıdır. Çalışmada kullanılan veri seti, Kaggle Brain Tumor Dataset olup dört sınıftan oluşmaktadır:

Glioma
Meningioma
Pituitary
No Tumor

Görüntüler üzerinde veri artırma (Data Augmentation) yöntemleri uygulanarak modelin genelleme yeteneği artırılmıştır. Ardından, Convolutional Neural Network (CNN) mimarisi tasarlanarak eğitim gerçekleştirilmiştir. Modelin performansı accuracy, precision, recall ve F1-score metrikleriyle değerlendirilmiştir. Detaylı teknik anlatım proje içerisinde yer almaktadır.

## Metrikler
Eğitim süreci sonunda model; eğitim verisinde yüksek bir başarı elde etmiş Train Accuracy ≈ 0.90, doğrulama verisinde ise Validation Accuracy ≈ 0.80 seviyesine ulaşmıştır. Train Loss değerinin sürekli azalmasına karşın Validation Loss dalgalı bir seyir izlemiş, bu da modelin kısmi bir overfitting eğiliminde olduğunu göstermiştir. Buna rağmen, test verisi üzerinde elde edilen yaklaşık %86 doğruluk oranı, modelin beyin tümörü sınıflandırmasında etkili bir performans sergilediğini ortaya koymaktadır. 
Metriklerin detaylı yorumları proje içerisinde yer almaktadır.

## Sonuç ve Gelecek Çalışmalar
Çalışma sonucunda geliştirilen model, eğitim ve doğrulama verileri üzerinde yüksek doğruluk elde etmiş olup test verisi üzerinde de güvenilir performans göstermiştir. Kullanılan veri artırma teknikleri sayesinde modelin farklı görüntü varyasyonlarına karşı daha dayanıklı öğrenmesi sağlanmıştır. Eğitim sırasında elde edilen doğruluk ve kayıp grafiklerinden, modelin aşırı öğrenme (overfitting) sorunu büyük ölçüde azaltılmıştır. Bu sonuçlar, CNN tabanlı yaklaşımların medikal görüntü analizi ve özellikle beyin tümörü tespiti için etkili bir yöntem olduğunu göstermektedir.

Gelecek çalışmalarda farklı hastanelerden ve cihazlardan elde edilen MR görüntüleri ile veri seti genişletilerek modelin genelleme yeteneği artırılabilir. Sınıflandırmanın yanı sıra tümörün boyut ve konumunu belirleyen segmentasyon modelleri ile bütünleşik bir sistem geliştirilebilir. Ayrıca modelin klinik ortamda hızlı ve güvenilir şekilde çalışabilmesi için optimize edilerek gerçek zamanlı beyin tümörü tespit sistemlerine entegre edilebilir.

### Proje ve Veri Seti
https://www.kaggle.com/code/dilandemirel/brain-tumor-detection
https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset
