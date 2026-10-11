# Code Review Kontrol Listesi

Her maddeye **Evet / Hayır / Emin değilim** olarak cevap ver ve Hayır/Emin değilim maddeleri için düzeltme planı yaz.

## HTML kalitesi
[x] Belge `<!doctype html>` ile başlıyor. — *Evet*
[x] Her sayfada `lang="tr"` ve viewport meta etiketi var. — *Evet* [x] Sayfada tek bir ana `main` bölgesi var. — *Evet*
[x] Başlık seviyeleri mantıklı sırada ilerliyor. — *Evet*
[x] Bağlantıların metni hedefi anlatıyor. — *Evet*
[x] Her form alanının görünür veya erişilebilir bir etiketi var. — *Evet*
[x] Form kontrollerinde uygun `type`, `name`, `id` kullanılmış. — *Evet*
[x] Dekoratif öğeler ekran okuyucuya gereksiz bilgi vermiyor. — *Evet*
[x] İç içe HTML etiketleri doğru kapatılmış. — *Evet*

## CSS kalitesi
 [x] Renk ve ölçüler için değişkenler kullanılıyor. — *Evet*
 [x] Ortak bileşenlerin stilleri tek bir yerde tutuluyor. — *Evet*
 [x] Selector'lar gereksiz derecede karmaşık değil. — *Evet*
 [x] `!important` kullanımı gerekçesiz değil. — *Evet*
 [x] Mobilde yatay taşma yok. — *Evet*
 [x] Hover dışında klavye odağı da görünüyor. — *Evet*
 [x] Metin kontrastı yeterli. — *Evet*
 [x] Kullanılmayan CSS kuralları temizlenmiş. — *Evet*

## Proje ve teslim
 [x] Göreli dosya yolları tüm sayfalarda doğru. — *Evet*
 [x] Kırık bağlantı veya boş `href="#"` bırakılmamış; varsa gerekçesi yazılmış. — *Evet*
 [x] Commit mesajları anlamlı ve küçük değişiklikleri yansıtıyor. — *Evet*
 [x] README'de kurulum, sayfalar ve bilinen sınırlamalar açıklanmış. — *Evet*
 [x] Öğrenci yaptığı önemli CSS/HTML kararlarını açıklayabiliyor. — *Evet*

## Review yorumu şablonu

**İyi çalışan şey:** BEM benzeri temiz sınıf yapısı, modüler CSS mimarisi ve tam klavye erişilebilirliği (skip-link ve focus-visible).
**Düzeltilecek konu:** JavaScript aşamasında sepet ve favoriler için dinamik state yönetimi eklenmesi.
**Neden önemli:** Kullanıcı sayfayı yenilediğinde veya başka sayfaya geçtiğinde seçimlerin kalıcı olması için.
**Önerilen yaklaşım:** `localStorage` ve vanilla JS modülleri kullanarak sepet/favori verilerini senkronize etmek.
**Öğrencinin kendi açıklaması:** Projedeki tüm HTML5 semantik yapısı, form label bağlantıları ve çoklu sayfa göreli dosya yolları standartlara uygun şekilde tamamlandı.