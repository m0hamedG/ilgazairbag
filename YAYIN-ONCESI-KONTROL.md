# Yayın Öncesi Kontrol Listesi

Site tamamen statik HTML + CSS + vanilla JS ile hazırlandı (build sistemi yok). Şu an GitHub Pages'te geçici adreste yayında:

👉 https://m0hamedg.github.io/ilgazairbag/

## ✅ Tamamlananlar

- **Logo**: Gerçek logo `images/logo.jpg` olarak eklendi, header/footer/favicon'da kullanılıyor.
- **Fotoğraflar**: Gerçek servis fotoğrafları (atölye, teknisyen, airbag/direksiyon/torpido/emniyet kemeri, X-431/Autel arıza tespit ekranları) `/images/` altına eklendi, tüm placeholder alanlar dolduruldu.
- **Telefon**: `+90 549 746 40 06` — tüm `tel:`/`wa.me` linklerine işlendi (WhatsApp'ın da aynı numara olduğu varsayıldı).
- **Adres**: "Oto San. Sit. 33. Sok. No:38, Şaşmaz, Ankara" — footer, iletişim sayfası ve schema.org verisine işlendi.
- **E-posta**: `ilgazairbag@gmail.com`.
- **Sosyal medya**: Instagram `instagram.com/ilgaz.airbag` olarak güncellendi, Facebook tamamen kaldırıldı.
- **Deneyim**: "10+ Yıllık Tecrübe", 2016 kuruluş yılı metne işlendi.
- **Hizmet isimleri**: "Torpido Tamiri" → "Torpido Kaplama ve Tamiri", "Direksiyon Airbagi" → "Airbag Ekspertiz" (görünen metinler güncellendi, dosya adları/URL'ler SEO kırılmasın diye aynı kaldı).
- **Dosya yolları**: Tüm iç linkler göreli (`css/style.css`, `../hizmetler/...` gibi) yazıldı — site herhangi bir alt klasörde (mevcut GitHub Pages adresi gibi) veya domain kökünde sorunsuz çalışır.
- **SEO adresleri**: robots.txt, sitemap.xml, rss.xml ve tüm sayfalardaki canonical/OG/JSON-LD URL'leri **geçici olarak** `https://m0hamedg.github.io/ilgazairbag/` adresine ayarlandı (Search Console kurulumu için).

## ⚠️ Hâlâ Placeholder / Eksik Olanlar

| Eksik | Nerede | Not |
|---|---|---|
| `[Pazartesi - Cumartesi 09:00 - 19:00]` | İletişim bölümleri | Gerçek çalışma saatleri girilmeli |
| `[POSTA KODU]` | index.html LocalBusiness JSON-LD | Posta kodu eksik |
| `https://formspree.io/f/[FORMSPREE_ID]` | İletişim formu | Formspree hesabı açıp ID girilmeli |
| `https://www.google.com/maps?q=Ilgaz%20Airbag...` | Harita gömme | Gerçek adresle/Google Maps "Yerleştir" koduyla değiştirilmeli |
| `images/og-cover.jpg` | Sosyal paylaşım kapak görseli | Henüz eklenmedi (1200x630 önerilir) |

## 🔴 Önemli: Özel Domain Alındığında Yapılacaklar

Şu an tüm canonical/OG/sitemap/robots URL'leri **geçici** GitHub Pages adresini (`m0hamedg.github.io/ilgazairbag`) gösteriyor. Gerçek bir alan adı (örn. `ilgazairbag.com`) alıp bağladığınızda:
1. Bu URL'lerin hepsinin gerçek domain'e güncellenmesi gerekir (toplu bul-değiştir ile hızlıca yapılabilir).
2. Google Search Console'a yeni domain'i ayrı bir mülk (property) olarak eklemek ve sitemap'i yeniden göndermek gerekir.
3. GitHub Pages ayarlarında Custom domain alanına yeni domain girilmeli.

## Diğer

- **Yasal sayfalar** (KVKK, Gizlilik, Çerez) genel şablon metinleridir — mevzuata tam uyum için hukuk danışmanına gösterilmesi önerilir.
