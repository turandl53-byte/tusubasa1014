 "Bu proje eğitim amaçlı yapılmış bir Twitter klonudur, ticari bir amacı yoktur"
# 🐦 Tvvitter

Yerel ağda çalışan, Twitter benzeri sosyal medya uygulaması.

## 🚀 Özellikler

- 🎨 Twitter birebir arayüz (beyaz tema)
- 🔒 Admin şifresi ile paylaşım yetkisi
- 🖼️ Resim paylaşımı
- 🎬 Video paylaşımı
- 👀 Şifresiz kullanıcılar sadece görüntüleyebilir
- 🤖 Otomatik sahte tweet akışı
- 🔍 Resim ve videoya tıklayınca büyütme
- 🌐 ngrok ile dünyaya açma desteği
- 💻 Tamamen local çalışır, veritabanı gerektirmez

## 📋 Gereksinimler

- Python 3.7+
- Flask

## ⚙️ Kurulum


# Projeyi klonla
git clone https://github.com/kullanici_adin/tvvitter.git
cd tvvitter

# Flask kur
pip install flask

# Sunucuyu başlat
python3 server.py


## 🌐Kurulum
Tarayıcıda aç: http://localhost:8080

Admin Paylaşımı
Admin şifresi: 12345

Şifreyi değiştirmek için server.py içinde ADMIN_SIFRE değişkenini düzenle

Ağdaki Diğer Cihazlardan Bağlanma


# IP adresini öğren
hostname -I

# Diğer cihazdan bağlan
http://192.168.x.x:8080
ngrok ile Dünyaya Açma
bash
ngrok http 8080


## 📁 Dosya Yapısı
text
tvvitter/
├── server.py          # Flask sunucu
├── requirements.txt   # Bağımlılıklar
├── README.md          # Bu dosya
├── static/
│   ├── resimler/      # Yüklenen resimler
│   └── videolar/      # Yüklenen videolar
└── templates/
    └── index.html     # Ana sayfa


🔧 Özelleştirme
Admin Şifresi Değiştirme
server.py dosyasında:

python
ADMIN_SIFRE = "yeni_sifre"
Sahte Tweet Sıklığı
server.py dosyasında:

python
time.sleep(90)  # 90 saniye, istediğin değeri yaz
Tema Değiştirme
index.html içindeki CSS renk kodlarını düzenle.


## 🛡️ Güvenlik

Sadece yerel ağda çalışır

Admin şifresi olmadan paylaşım yapılamaz

Veritabanı yok, sunucu kapanınca her şey silinir

📝 Lisans
MIT

Geliştirici: [tusubasa1014]

Yapım Tarihi: 2026


