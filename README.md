# Yapay Sinir Ağı (ANN) Kullanarak Kalp Hastalığı Tahmini

Bu depo, TensorFlow ve Keras ile Yapay Sinir Ağı (ANN) kullanarak kalp hastalığını tahmin eden bir projeyi içermektedir. Kullanılan veri seti Kaggle'dan alınan "Heart Disease UCI" veri setidir.

## İçindekiler

- [Giriş](#giriş)
- [Veri Seti](#veri-seti)
- [Kurulum](#kurulum)
- [Kullanım](#kullanım)
- [Model Mimarisi](#model-mimarisi)
- [Sonuçlar](#sonuçlar)
- [Katkıda Bulunma](#katkıda-bulunma)
- [Lisans](#lisans)

## Giriş

Kalp hastalığı dünya çapında büyük bir sağlık sorunudur ve erken teşhis hayat kurtarabilir. Bu proje, çeşitli tıbbi özelliklere dayalı olarak hastalarda kalp hastalığının varlığını tahmin etmek için bir Yapay Sinir Ağı (ANN) kullanmaktadır.

## Veri Seti

Bu proje için kullanılan veri seti, [Kaggle](https://www.kaggle.com/ronitf/heart-disease-uci) üzerinde bulunan "Heart Disease UCI" veri setidir. Veri seti 303 örnek ve yaş, cinsiyet, kan basıncı, kolesterol seviyeleri gibi 14 özellik içermektedir.

## Kurulum

Bu projeyi çalıştırmak için Python ve aşağıdaki kütüphanelerin yüklü olması gerekmektedir:

- TensorFlow
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

Bu kütüphaneleri `pip` kullanarak yükleyebilirsiniz:

```bash
pip install tensorflow numpy pandas scikit-learn matplotlib

## Model Mimarisi
Bu projede kullanılan ANN modelinin mimarisi aşağıdaki gibidir:

Girdi Katmanı: 13 nöron (her özellik için bir)
Gizli Katman 1: 16 nöron, ReLU aktivasyonu
Dropout Katmanı: %50 dropout oranı
Gizli Katman 2: 32 nöron, ReLU aktivasyonu
Dropout Katmanı: %50 dropout oranı
Çıktı Katmanı: 1 nöron, Sigmoid aktivasyonu
Model, Adam optimizasyon yöntemi ve binary crossentropy kayıp fonksiyonu ile derlenmiştir. 50 epoch boyunca, 10'luk batch boyutu ile eğitilmiştir.

## Sonuçlar
Modelin performansı doğruluk, karışıklık matrisi ve sınıflandırma raporu kullanılarak değerlendirilmiştir. Eğitim epochları boyunca doğruluk ve kayıp grafikleri de görselleştirilmiştir.


## Katkıda Bulunma
Katkılar memnuniyetle karşılanır! Herhangi bir geliştirme veya öneriniz varsa, lütfen bir sorun oluşturun veya bir pull request gönderin.
