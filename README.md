```markdown
# TYT Deneme Modülü

![License](https://img.shields.io/badge/license-Proprietary-blue.svg)
![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)
![Version](https://img.shields.io/badge/version-1.0.0-yellow.svg)

## İçindekiler
- [Proje Adı](#proje-adı)
- [Proje Açıklaması](#proje-açıklaması)
- [Kullanılan Teknolojiler](#kullanılan-teknolojiler)
- [Özellikler](#özellikler)
- [Kurulum](#kurulum)
- [Kullanım](#kullanım)
- [Dosya Yapısı](#dosya-yapısı)
- [Güvenlik](#güvenlik)
- [Lisans](#lisans)
- [İletişim](#iletişim)

## Proje Adı
**TYT Deneme Modülü**

## Proje Açıklaması
TYT Deneme Modülü, öğrencilerin TYT sınavına hazırlık sürecinde performanslarını takip etmelerini ve değerlendirmelerini sağlayan web tabanlı bir sistemdir. Kullanıcılar, telefon numaralarını girerek sınav sonuçlarına erişebilir, detaylı analizler ve grafiklerle performanslarını gözlemleyebilirler.

## Kullanılan Teknolojiler
- **Frontend:**
  - HTML5
  - CSS3
  - JavaScript
  - Chart.js
- **Backend:**
  - PHP
  - MySQL
- **Diğer:**
  - Composer
  - Modern web teknolojileri ve kütüphaneleri

## Özellikler
- **Sonuç Sorgulama:** Telefon numarası girilerek sınav sonuçlarına hızlı erişim.
- **Detaylı Analizler:** Doğru, yanlış ve net sayılarıyla birlikte detaylı performans analizi.
- **Grafiksel Görselleştirme:** TYT puanları, net analizleri ve sıralama analizlerini görsel grafiklerle sunma.
- **Sınav Seçimi:** Farklı deneme sınavlarının sonuçlarını karşılaştırma imkanı.
- **Kullanıcı Dostu Arayüz:** Basit ve anlaşılır tasarım ile kolay kullanım.

## Kurulum
### Ön Koşullar
- PHP 7.4 veya üzeri
- MySQL Veritabanı
- Web Sunucusu (Apache veya Nginx)
- Composer Paket Yöneticisi

### Adım Adım Kurulum
1. **Depoyu Klonlayın:**
    ```bash
    git clone https://github.com/kullanici/tytdeneme_modulu.git
    ```
2. **Gerekli Bağımlılıkları Yükleyin:**
    ```bash
    cd tytdeneme_modulu
    composer install
    ```
3. **Veritabanını Ayarlayın:**
    - `api.php` dosyasında veritabanı bağlantı bilgilerini güncelleyin.
    - Gerekli veritabanı tablolarını oluşturun.
4. **Web Sunucusunu Yapılandırın:**
    - Proje dizinini web sunucunuzun kök dizini olarak ayarlayın.
    - Gerekli izinleri verin.
5. **Uygulamayı Başlatın:**
    - Web tarayıcınızda projenin URL'sine giderek uygulamayı kullanmaya başlayın.

## Kullanım
1. **Telefon Numarası Girin:**
    - Ana sayfada bulunan arama kutusuna telefon numaranızı girin (örnek: `5XX XXX XX XX`).
2. **Sonuçları Görüntüleyin:**
    - "Sorgula" butonuna tıklayarak sınav sonuçlarını görüntüleyin.
3. **Analizleri İnceleyin:**
    - Öğrenci bilgileri, sınav sıralamaları ve ders bazlı net analizlerini inceleyin.
    - Grafik sekmelerinden performansınızı görsel olarak analiz edin.
4. **Sınav Seçimi Yapın:**
    - Farklı deneme sınavlarını seçerek performansınızı karşılaştırın.

![Uygulama Ekran Görüntüsü](path/to/screenshot.png)

## Dosya Yapısı
```
tytdeneme_modulu/
├── api/
│   └── api.php             # API endpoint'leri
├── cache/                  # Önbellek dosyaları
├── js/
│   ├── tytChart.js         # TYT Puanları Grafiği
│   ├── turkceNetChart.js   # Türkçe Net Grafiği
│   ├── sosyalNetChart.js   # Sosyal Net Grafiği
│   ├── matematikNetChart.js# Matematik Net Grafiği
│   ├── fenNetChart.js      # Fen Net Grafiği
│   ├── personalNetAnalysisChart.js    # Kişisel Net Analizi Grafiği
│   ├── personalRankAnalysisChart.js   # Kişisel Sıralama Analizi Grafiği
│   └── personalScoreAnalysisChart.js  # Kişisel Puan Analizi Grafiği
├── vendor/                 # Composer bağımlılıkları
├── exports/                # Dışa aktarım dosyaları
├── logs/                   # Log dosyaları
├── index.html              # Ana HTML dosyası
├── style.css               # Genel stil dosyası
├── mobile-table-fix.css    # Mobil tablo düzenleme stil dosyası
├── chart-styles.css        # Grafik stil dosyası
├── ranking-tables.css      # Sıralama tabloları stil dosyası
└── README.md               # Bu dosya
```

- **api/**: API endpoint'lerinin bulunduğu klasör.
- **js/**: JavaScript dosyalarının bulunduğu klasör.
- **vendor/**: Composer ile yüklenen bağımlılıkların bulunduğu klasör.
- **exports/**: Dışa aktarım işlemleri için kullanılan dosyalar.
- **logs/**: Uygulama loglarının tutulduğu klasör.
- **index.html**: Uygulamanın ana HTML dosyası.
- **style.css**: Uygulamanın genel stil dosyası.
- **mobile-table-fix.css**: Mobil cihazlar için tablo düzenlemeleri.
- **chart-styles.css**: Grafiklerin stil ayarları.
- **ranking-tables.css**: Sıralama tablolarının stil ayarları.

## Güvenlik
- **Yetkilendirme:** Sistem, sadece yetkili kullanıcıların erişimine izin verir.
- **Veri Şifreleme:** Tüm hassas veriler şifreli olarak saklanır.
- **Güncellemeler:** Yazılım düzenli olarak güvenlik yamaları ve güncellemeleri ile güncellenir.
- **Veritabanı Güvenliği:** SQL enjeksiyonlarına karşı önlemler alınmıştır.

## Lisans
Bu proje özel lisanslıdır ve tüm hakları saklıdır. Kaynak kodunun kopyalanması, dağıtılması veya değiştirilmesi yasaktır.

## İletişim
Projeyle ilgili sorularınız veya geri bildirimleriniz için lütfen aşağıdaki iletişim bilgilerinden bana ulaşın:

- **İsim:** [Adınız Soyadınız]
- **Email:** [email@example.com]
- **LinkedIn:** [linkedin.com/in/adiniz](https://linkedin.com/in/adiniz)

---

© 2025 TYT Deneme Modülü. Tüm hakları saklıdır.
```

---

### Açıklama

- **Başlık ve Rozetler:** Proje adı ve lisans, sürüm bilgileri gibi önemli bilgiler rozetlerle belirtilmiştir.
- **İçindekiler:** README'nin büyük olması durumunda kullanıcıların kolayca gezinmesini sağlar.
- **Proje Açıklaması:** Projenin amacı ve temel işlevleri hakkında kısa ve net bir özet sunar.
- **Kullanılan Teknolojiler:** Projede kullanılan tüm teknolojiler madde işaretleriyle listelenmiştir.
- **Özellikler:** Projenin sunduğu ana özellikler ayrıntılı olarak açıklanmıştır.
- **Kurulum:** Projeyi yerel ortamda çalıştırmak için gereken adımlar detaylandırılmıştır.
- **Kullanım:** Uygulamanın nasıl kullanılacağı adım adım anlatılmıştır.
- **Dosya Yapısı:** Projenin klasör ve dosya yapısı şematik olarak gösterilmiştir.
- **Güvenlik:** Projenin güvenlik önlemleri hakkında bilgi verilmiştir.
- **Lisans:** Projenin lisans durumu açıkça belirtilmiştir.
- **İletişim:** Kullanıcıların proje hakkında daha fazla bilgi alabilecekleri iletişim bilgileri sağlanmıştır.

### Ek İpuçları

- **Ekran Görüntüleri:** `![Uygulama Ekran Görüntüsü](path/to/screenshot.png)` etiketi ile projeye ait ekran görüntülerini README'ye ekleyebilirsiniz. Bu görselleri projenizin `images/` klasörüne koyup yolunu güncelleyebilirsiniz.
- **Videolar:** Projeyi tanıtan kısa videolar varsa, README'ye ekleyerek kullanıcı deneyimini artırabilirsiniz.
- **Bağlantılar:** README'deki bağlantıları (örneğin, LinkedIn profili, dokümantasyon) güncel ve doğru URL'lerle değiştirdiğinizden emin olun.

Bu README.md dosyasını projenizin kök dizininde `README.md` adıyla oluşturabilir ve gerektiğinde özelleştirebilirsiniz. Eğer eklemek istediğiniz başka bölümler veya değişiklikler varsa, lütfen bana bildirin.
