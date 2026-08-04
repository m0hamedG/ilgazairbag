# Yayın Öncesi Kontrol Listesi

Site tamamen statik HTML + CSS + vanilla JS ile hazırlandı (build sistemi yok).

## ✅ Tamamlananlar

- **Logo**: Paylaştığınız logo `/images/logo.jpg` olarak eklendi, header/footer/favicon'da kullanılıyor.
- **Fotoğraflar**: Downloads klasöründeki gerçek WhatsApp servis fotoğrafları (12 adet, kategori bazında seçilerek) `/images/` altına kopyalandı ve tüm `img-placeholder` blokları bunlarla değiştirildi. Hero arka planı da artık gerçek bir fotoğraf (araç iç mekanı).
- **Telefon**: `+90 549 746 40 06` — tüm `tel:`/`wa.me` linklerine ve görünen metinlere işlendi.
  - **Varsayım**: WhatsApp numarası da aynı numara olarak ayarlandı. Farklıysa bildirin.
- **Adres**: "Oto San. Sit. 33. Sok. No:38, Şaşmaz, Ankara" — footer, iletişim sayfası ve schema.org verisine işlendi.
- **Hizmet isimleri**: "Torpido Tamiri" → "Torpido Kaplama ve Tamiri", "Direksiyon Airbagi" → "Airbag Ekspertiz" olarak güncellendi (başlıklar, kartlar, footer linkleri, sayfa içerikleri). **Not**: Dosya adları/URL'ler değiştirilmedi (`/hizmetler/torpido-tamiri.html`, `/hizmetler/direksiyon-airbagi.html` aynı kaldı) — SEO/link kırılmasını önlemek için. URL'lerin de değişmesini isterseniz söyleyin.
  - Ürünler bölümündeki "Direksiyon" ve "Torpido" kategori sayfalarının kendi başlıkları (`urunler/direksiyon.html`, `urunler/torpido.html`) bilinçli olarak değiştirilmedi, sadece footer linkleri güncellendi — bunlar ayrı bir ürün kategorisi, hizmet adıyla karıştırılmasın diye.

## ⚠️ Hâlâ Placeholder Olanlar

| Placeholder | Nerede | Not |
|---|---|---|
| `info@ilgazairbag.com` (mailto) / `[E-POSTA ADRESİ]` | İletişim, footer | Gerçek e-posta adresinizi verin |
| `[Pazartesi - Cumartesi 09:00 - 19:00]` | İletişim bölümleri | Gerçek çalışma saatleri |
| `[POSTA KODU]`, addressLocality/Region | index.html LocalBusiness JSON-LD | Posta kodu eksik |
| `https://formspree.io/f/[FORMSPREE_ID]` | İletişim formu | Formspree hesabı açıp ID girilmeli |
| `https://www.google.com/maps?q=Ilgaz%20Airbag...` | Harita gömme | Gerçek adresle/Google Maps "Yerleştir" koduyla değiştirilmeli |
| `instagram.com/ilgazairbag`, `facebook.com/ilgazairbag` | Footer sosyal linkler | Gerçek hesap adresleri doğrulanmalı |
| `/images/og-cover.jpg` | Sosyal paylaşım kapak görseli | Henüz eklenmedi (1200x630 önerilir) |
| `https://www.ilgazairbag.com` | Tüm canonical/OG/sitemap | Gerçek domain farklıysa toplu değiştirilmeli |

## Diğer

- **Yasal sayfalar** (KVKK, Gizlilik, Çerez) genel şablon metinleridir — mevzuata tam uyum için hukuk danışmanına gösterilmesi önerilir.
- **Hosting**: Tüm linkler root-relative (`/css/style.css`) yazıldı; siteyi bir alt klasörde değil domain kökünde yayınlayın (GitHub Pages proje sayfası kullanacaksanız yolları güncellemeniz gerekir).
- **UI kütüphanesi (21st.dev) sorunuz**: Ayrı olarak yanıtlandı, bkz. sohbet.
