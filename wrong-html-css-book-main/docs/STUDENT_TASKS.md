# Öğrenci Görevleri

## Zorunlu görevler

1. Ana sayfadaki hero başlığını kendi metninle değiştir; anlamlı satır kırılımlarını koru.
2. Kataloğa iki kitap ekle. Her kartın kategori, başlık, yazar, fiyat ve puan alanları olsun.
3. Katalog sayfasına “En çok satanlar” ve “Yeni çıkanlar” bölümleri ekle.
4. İletişim formuna telefon alanı ve tercih edilen iletişim yöntemi seçimi ekle.
5. Giriş formuna “Beni hatırla” checkbox'ı ekle. Şimdilik davranışını açıklayan not bırak.
6. Ürün kartlarına indirimli fiyat gösterimi ekle. Eski fiyatı semantik olarak uygun biçimde işaretle.
7. Footer'a teslimat, iade ve gizlilik sayfalarına giden bağlantılar ekle. Bu sayfaları da oluştur.
8. Tüm sayfalardaki header/footer bağlantılarını tutarlı hâle getir.
9. Responsive testlerini yap ve bulunan sorunları `docs/RESPONSIVE_TESTS.md` dosyasına kaydet.
10. `README.md` dosyasını kendi projenin gerçek durumuna göre güncelle.

## Teslim formatı

- GitHub deposu bağlantısı
- 1440px masaüstü ekran görüntüsü
- 390px mobil ekran görüntüsü
- `docs/RESPONSIVE_TESTS.md`
- 3 zorlandığın nokta ve bunları nasıl çözdüğün
- Code review checklist

## Bonus görevler

- [X] CSS ile açılır kategori navigasyonu tasarla (JavaScript olmadan erişilebilirlik sınırlarını not et).
- [X] “Okuma listesi” sayfası ekle.
- [X] Ürün kartına stok durumu rozeti ekle.
- [X] Tasarım token'larını `variables.css` içinde gruplandır.
- [x] Koyu tema için ayrı bir CSS değişken seti tasarla; yalnızca CSS ile tema değiştirmenin sınırlarını açıkla. *Cevap:  **Yalnızca CSS ile Tema Değiştirmenin Sınırları:**
 1. **Kalıcılık yoktur:** Sayfa yenilenince (`F5`) veya başka sayfaya geçince tema sıfırlanır (hafızada tutmak için JavaScript/localStorage gerekir).
2. **Sisteme bağlıdır:** `@media (prefers-color-scheme: dark)` sadece cihazın ayarlarına bakar, kullanıcının site içi butonla manuel ve kalıcı seçim yapmasına izin vermez.
 3. **Görseller değişmez**: CSS değişkenleri renkleri değiştirir ama `<img>` etiketindeki resimleri veya logoları dinamik olarak değiştiremez.
- [x] Bir `404.html` hata sayfası oluştur.
- [x] Görsel varlıklar için `assets/images/` içinde bir kaynak ve lisans notu dosyası hazırla.
- [x] Lighthouse veya benzeri bir araçla erişilebilirlik ve performans kontrolü yap; sonucu raporla.
