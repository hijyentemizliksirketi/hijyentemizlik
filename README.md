# Hijyen Temizlik — Gaziantep

> **Kusursuz hijyen, profesyonel standart.**

Gaziantep merkezli profesyonel temizlik ve hijyen şirketi **Hijyen Temizlik** için geliştirilen kurumsal web sitesi.

![Durum](https://img.shields.io/badge/durum-yayında-success) ![Platform](https://img.shields.io/badge/platform-Vercel-000) ![Tür](https://img.shields.io/badge/tür-Statik%20Site-2E90FA)

## ✨ Özellikler

- Tamamen tek dosyalık, bağımlılıksız statik site (HTML + CSS + vanilla JS)
- Premium ajans seviyesi tasarım: preloader, marquee, parallax, sticky bölümler, 3D tilt, magnetic butonlar
- 13 hizmet kartı — her biri hizmete özel ön-dolu WhatsApp mesajıyla `+90 553 985 22 74` numarasına yönlendirir
- Ücretsiz teklif formları (hero + iletişim) → doğrudan WhatsApp'a mesaj iletir
- SSS akordiyonu, galeri, müşteri referansları, çalışma alanları (Gaziantep + 8 ilçe)
- **Tam kapsamlı SEO**: Schema.org `@graph` (LocalBusiness + WebSite + FAQPage, 13 hizmetli OfferCatalog), robots.txt, sitemap.xml, OG/Twitter kartları, canonical, geo meta'ları
- Erişilebilirlik: semantik HTML, tek `h1`, skip-link, aria özellikleri, `prefers-reduced-motion` desteği
- Mobil uyumlu, Google Fonts (Sora / Inter / Fraunces)

## 📁 Proje Yapısı

```
.
├── index.html            # Ana sayfa (tüm site tek dosyada)
├── assets/
│   ├── hero.jpg          # Hero arka plan görseli
│   ├── team.jpg          # Ekip fotoğrafı
│   ├── detail.jpg        # Endüstriyel ekipman detayı
│   ├── space.jpg         # Kurumsal tesis görseli
│   ├── og-image.jpg      # Sosyal paylaşım (OG) görseli 1200×630
│   └── apple-touch-icon.png
├── 404.html              # Özel 404 sayfası
├── robots.txt            # Arama motoru yönergeleri
├── sitemap.xml           # Site haritası
└── vercel.json           # Vercel dağıtım yapılandırması
```

## 🚀 Yerel Çalıştırma

```bash
# Python
python3 -m http.server 8080

# veya Node
npx serve .
```

Tarayıcıda `http://localhost:8080` adresini açın.

## ☁️ Vercel'e Dağıtım

### Yöntem 1: GitHub üzerinden (önerilen)
1. Bu repo'yu Vercel'de **Add New → Project** ile bağlayın.
2. Framework: **Other** seçin, **Deploy** butonuna basın.
3. Her `main` dalına push yaptığınızda site otomatik güncellenir.

### Yöntem 2: Vercel CLI
```bash
npm i -g vercel
vercel          # önizleme URL'i
vercel --prod   # canlı yayına alma
```

> ⚠️ **Alan adı notu:** `index.html` (head içindeki SEO bloğu), `sitemap.xml` ve `robots.txt` dosyalarında
> `hijyentemizlik.com` placeholder olarak kullanılmıştır. Resmi alan adınızı aldığınızda bu üç dosyada
> ve `index.html` içindeki JSON-LD bloğunda adresi kendi domain'inizle değiştirin.

## 🌐 Domain Bağlama

1. Vercel → Proje → **Settings → Domains** → kendi `.com` domain'inizi ekleyin.
2. DNS sağlayıcınızda Vercel'in gösterdiği `CNAME` kaydını oluşturun
   (ör. `www → cname.vercel-dns.com`).
3. DNS yayılmasının ardından (dakikalar–24 saat) `https://domaininiz.com` aktif olur.
   Vercel SSL sertifikasını otomatik ve ücretsiz üretir.

## 📞 İletişim

- **Telefon / WhatsApp:** +90 553 985 22 74
- **Konum:** Gaziantep, Türkiye — Merkez ve Tüm İlçeler
- **Çalışma saatleri:** 7/24

## 📄 Lisans

Tüm hakları saklıdır — © Hijyen Temizlik.
