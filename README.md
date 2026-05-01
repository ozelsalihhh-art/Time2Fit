# Time2Fit 👔

> **Kombin değil, strateji.**

Capsule wardrobe mantığıyla dolabını yönet. Kıyafetlerini kaydet, kombinlerini keşfet, gerçek ihtiyacına göre alışveriş yap. **Gemini AI** ile kişiselleştirilmiş kombin önerileri, **Pinterest & Google Images** entegrasyonuyla ilham al.

---

## Nedir?

Time2Fit, tek bir HTML dosyasından çalışan, internet bağlantısı gerektirmeyen bir kişisel dolap yönetim uygulamasıdır. Kural tabanlı renk uyum motoru ve capsule wardrobe ilkeleriyle dolabını analiz eder, kombin önerir ve alım kararlarında rehberlik eder.

---

## Özellikler

### 👔 Dolap
- Kıyafet ekleme — fotoğraf opsiyonel
- 2 seviyeli kategori sistemi (Üst Giyim → Gömlek, T-Shirt, Polo...)
- Renk seçici (16 renk, Türkçe isimli)
- Sezon, ortam, marka, fiyat bilgisi
- Arama ve kategori filtresi
- Uzun basarak düzenle / sil

### 🎲 Kombin
- Renk uyum matrisi ile otomatik kombin önerisi
- **Günlük** ve **Smart Casual** filtresi
  - Günlük → ceketsiz, rahat kombinler
  - Smart Casual → ceket zorunlu, ofis uyumlu
- Her kombinasyonda renk uyum yüzdesi
- Yenile ile farklı kombinler
- **📌 Pinterest** ve **🔍 Google Images** butonu — kombini gerçek kıyafetlerde gör

### 📊 Analiz
- Capsule Skoru (100 üzerinden)
  - Renk Uyumu
  - Kategori Dengesi
  - Kombinasyon Gücü
- Dolap yorumları (akıllı tespitler)
- Unlock Piece — hangi parçayı eklersen en fazla kombin açılır

### ✨ Stil
- Renk Motoru — dolabındaki renkler + eksik renk önerileri
- Alım Kararı Asistanı — almayı düşündüğün parça gerçekten eksik mi?

### 🤖 AI Asistan
- Gemini AI ile kişiselleştirilmiş kombin önerileri
- Dolabındaki gerçek parça isimleriyle öneri
- Hazır hızlı aksiyonlar:
  - 🎲 Bugünkü kombin
  - 📅 Haftalık 7 günlük plan
  - 📊 Dolap analizi
  - 🛍️ Ne almalıyım?
  - 🏢 Ofis kombinleri
  - 😎 Hafta sonu stili
- Serbest soru sorma imkânı
- Son 10 soru geçmişi

### ⚙️ Ayarlar
- Dolap özeti (parça, kombin, toplam değer)
- Veri dışa aktar (JSON)
- Veri içe aktar (JSON)
- Gemini API anahtarı yönetimi
- Mayıs/Yaz Smart Casual Erkek Stil Rehberi
- Tüm verileri sil

---

## Kurulum

Herhangi bir kurulum gerekmez. `time2fit_v10.html` dosyasını tarayıcıda aç, kullanmaya başla.

Tüm veriler tarayıcının `localStorage` alanında saklanır.

---

## AI Asistan Kurulumu

AI Asistan özelliği için ücretsiz bir Gemini API anahtarı gereklidir.

### Adım 1 — API Anahtarı Al

1. [aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey) adresine git
2. Google hesabınla giriş yap
3. **"Create API key"** → **"Create API key in new project"** seç
4. Oluşturulan `AIza...` ile başlayan anahtarı kopyala

> **Not:** Yeni proje oluşturmanı öneririz. Yeni AI Studio projesi ücretsiz tier limitleriyle gelir, mevcut Google Cloud projesine bağlamak ek kota gerektiriyor.

### Adım 2 — Anahtarı Uygulamaya Gir

Dosyayı ilk açtığında otomatik olarak anahtar sorulur. Daha sonra değiştirmek istersen:

**Ayarlar → AI Asistan → Gemini API Anahtarını Değiştir**

Anahtarı girdikten sonra **"Tara"** butonuna bas — uygulama kullanılabilir modeli otomatik bulur ve kaydeder.

### Ücretsiz Kullanım Limitleri

| Model | İstek/Dakika | İstek/Gün |
|-------|-------------|-----------|
| gemini-2.0-flash-lite | 30 | 1.500 |
| gemini-2.0-flash | 15 | 1.500 |

Kişisel kullanım için günlük 1.500 istek fazlasıyla yeterlidir.

---

## Telefona Kurulum (PWA)

**iPhone (Safari):**
1. Dosyayı Safari'de aç
2. Alt menüden "Paylaş" butonuna bas
3. "Ana Ekrana Ekle" seçeneğini seç

**Android (Chrome):**
1. Dosyayı Chrome'da aç
2. Sağ üstteki menüden "Ana ekrana ekle" seçeneğini seç

Kurulumdan sonra uygulama tam ekran ve offline çalışır. (AI Asistan ve görsel arama özellikleri internet bağlantısı gerektirir.)

---

## Veri Yedekleme

Telefon değiştirmeden veya tarayıcı verilerini silmeden önce:

1. **Ayarlar** sekmesine git
2. **Veriyi Dışa Aktar** butonuna bas
3. JSON dosyasını güvenli bir yere kaydet

Geri yüklemek için **Veriyi İçe Aktar** butonunu kullan.

---

## Teknik Detaylar

- Tek HTML dosyası — framework yok, build süreci yok
- Sıfır bağımlılık — CDN'den font dışında hiçbir şey çekilmez
- Offline çalışır (AI Asistan ve görsel arama hariç)
- localStorage ile kalıcı veri
- 16×16 renk uyum matrisi (renk teorisi tabanlı)
- Capsule wardrobe kombin motoru
- Gemini API entegrasyonu
- Pinterest & Google Images arama entegrasyonu

---

## Geliştirme Notları

| Versiyon | İçerik |
|----------|--------|
| v1 | Temel yapı, Mint & Clay tema, kıyafet ekleme |
| v2 | Alt kategoriler |
| v3 | SVG logo, font güncellemesi |
| v4 | Capsule Skoru, Unlock Piece, Renk Motoru, Alım Kararı, Düzenle/Sil |
| v5 | Kombin Motoru, Ayarlar, Veri Yedekleme, Stil Rehberi |
| v6 | AI Asistan (Gemini API), haftalık plan, dolap analizi, API key yönetimi |
| v7–v9 | Kombin motoru iyileştirmeleri, Günlük/Smart Casual ayrımı, ceket zorunluluğu |
| v10 | Pinterest & Google Images entegrasyonu, İngilizce kombin arama promptu |

---

*Time2Fit — kişisel kullanım için geliştirilmiştir.*
