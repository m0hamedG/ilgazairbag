# Yayın Öncesi Kontrol Listesi

Site tamamen statik HTML + CSS + vanilla JS ile hazırlandı (build sistemi yok). Domain: **www.ilgazairbag.com** (canonical/OG/sitemap/robots hepsi bu adrese göre ayarlandı, CNAME dosyası eklendi).

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
- **SEO adresleri**: robots.txt, sitemap.xml, rss.xml ve tüm sayfalardaki canonical/OG/JSON-LD URL'leri `https://www.ilgazairbag.com/` adresine güncellendi.
- **CNAME**: GitHub Pages'in domain'i tanıması için repo köküne `CNAME` dosyası eklendi (içeriği: `www.ilgazairbag.com`).

## ⚠️ Hâlâ Placeholder / Eksik Olanlar

| Eksik | Nerede | Not |
|---|---|---|
| `[Pazartesi - Cumartesi 09:00 - 19:00]` | İletişim bölümleri | Gerçek çalışma saatleri girilmeli |
| `[POSTA KODU]` | index.html LocalBusiness JSON-LD | Posta kodu eksik |
| `https://formspree.io/f/[FORMSPREE_ID]` | İletişim formu | Formspree hesabı açıp ID girilmeli |
| `https://www.google.com/maps?q=Ilgaz%20Airbag...` | Harita gömme | Gerçek adresle/Google Maps "Yerleştir" koduyla değiştirilmeli |
| `images/og-cover.jpg` | Sosyal paylaşım kapak görseli | Henüz eklenmedi (1200x630 önerilir) |

## 🔴 Domain Bağlama — Yapılacaklar (DNS + GitHub Pages)

1. **DNS ayarları** (domain'i aldığınız yerde, örn. Natro/GoDaddy/Cloudflare paneli):
   - `www` için CNAME kaydı → `m0hamedg.github.io`
   - Kök domain (`ilgazairbag.com`, "@" ile gösterilir) için 4 adet A kaydı → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
2. **GitHub Pages ayarları**: Settings → Pages → Custom domain kutusuna `www.ilgazairbag.com` yazıp Save. DNS yayılması birkaç dakika–birkaç saat sürebilir.
3. **HTTPS**: DNS doğrulandıktan sonra "Enforce HTTPS" kutusu otomatik aktif olur (sertifika üretimi biraz zaman alabilir).
4. **Google Search Console**: `www.ilgazairbag.com` için yeni bir mülk (property) açılmalı, sitemap (`sitemap.xml`) yeniden gönderilmeli. Önceki geçici GitHub Pages adresi (m0hamedg.github.io/ilgazairbag) için mülk açtıysanız o ayrı kalır, artık kullanılmayacak.

## Diğer

- **Yasal sayfalar** (KVKK, Gizlilik, Çerez) genel şablon metinleridir — mevzuata tam uyum için hukuk danışmanına gösterilmesi önerilir.
