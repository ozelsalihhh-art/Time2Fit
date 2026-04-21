# Time2Fit 👔

> **Kombin değil, strateji.**

Capsule wardrobe mantığıyla dolabını yönet. Kıyafetlerini kaydet, kombinlerini keşfet, gerçek ihtiyacına göre alışveriş yap.

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
- Günlük / Smart Casual / Formal filtresi
- Her kombinasyonda renk uyum yüzdesi
- Yenile ile farklı kombinler

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

### ⚙️ Ayarlar
- Dolap özeti (parça, kombin, toplam değer)
- Veri dışa aktar (JSON)
- Veri içe aktar (JSON)
- Mayıs/Yaz Smart Casual Erkek Stil Rehberi
- Tüm verileri sil

---

## Kullanım

Herhangi bir kurulum gerekmez. `time2fit_v5.html` dosyasını tarayıcıda aç, kullanmaya başla.

Tüm veriler tarayıcının `localStorage` alanında saklanır.

---

## Telefona Kurulum (PWA)

**iPhone (Safari):**
1. Dosyayı Safari'de aç
2. Alt menüden "Paylaş" butonuna bas
3. "Ana Ekrana Ekle" seçeneğini seç

**Android (Chrome):**
1. Dosyayı Chrome'da aç
2. Sağ üstteki menüden "Ana ekrana ekle" seçeneğini seç

Kurulumdan sonra uygulama tam ekran ve offline çalışır.

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
- Offline çalışır
- localStorage ile kalıcı veri
- 16×16 renk uyum matrisi (renk teorisi tabanlı)
- Capsule wardrobe kombin motoru

---

## Geliştirme Notları

Proje part part geliştirildi:

| Versiyon | İçerik |
|----------|--------|
| v1 | Temel yapı, Mint & Clay tema, kıyafet ekleme |
| v2 | Alt kategoriler |
| v3 | SVG logo, font güncellemesi |
| v4 | Capsule Skoru, Unlock Piece, Renk Motoru, Alım Kararı, Düzenle/Sil |
| v5 | Kombin Motoru, Ayarlar, Veri Yedekleme, Stil Rehberi |

---

*Time2Fit — kişisel kullanım için geliştirilmiştir.*
