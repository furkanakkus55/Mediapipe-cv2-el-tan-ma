# El Takip Sistemi (Python, OpenCV, MediaPipe)

Bu proje, Python programlama dili kullanılarak geliştirdiğim gerçek zamanlı bir el takip sistemidir. El tespiti için Google tarafından geliştirilen güçlü bir kütüphane olan **MediaPipe**'i, görüntü işleme için ise **OpenCV**'yi kullandım. Bu sistem, kameradan alınan canlı görüntü üzerinden bir veya iki elin konumunu algılayıp, parmak kemik bağlantılarını ve parmak uçlarını görsel olarak işaretler. Aynı zamanda sistemin ne kadar hızlı çalıştığını anlamak için gerçek zamanlı FPS (Frame Per Second) bilgisi de ekrana yazdırılır.

## Amaç

Bu projeyi geliştirirken amacım, görüntü işleme ve yapay zeka temelli el tespiti konularında hem kendimi geliştirmek hem de pratikte kullanılabilir bir uygulama ortaya koymaktı. Aynı zamanda bu proje sayesinde:
- MediaPipe gibi hazır modellerle nasıl çalışılacağını öğrendim.
- OpenCV'nin kamera ve görüntü işleme fonksiyonlarını detaylı şekilde kullanmayı deneyimledim.
- Gerçek zamanlı sistemlerde performans ölçümü (FPS) gibi kavramları pratiğe döktüm.

## Özellikler

- Gerçek zamanlı el algılama (maksimum 2 el)
- Parmak uçlarının ve kemik bağlantı noktalarının çizimi
- Aynalı kamera görünümü (daha doğal kullanıcı deneyimi için)
- Anlık FPS değeri (performans kontrolü için)
- `q` tuşuna basarak hızlı ve sorunsuz çıkış

## Kullanılan Teknolojiler

- **Python 3.7+**: Proje dili
- **OpenCV**: Görüntü yakalama, dönüştürme, ekrana yazdırma
- **MediaPipe (Hands)**: El algılama ve anahtar nokta çıkarımı
- **time** modülü: FPS hesaplaması için

## Gereksinimler

Bu projeyi çalıştırmak için aşağıdaki Python kütüphanelerinin sisteminizde kurulu olması gerekir:

```bash
pip install opencv-python mediapipe
