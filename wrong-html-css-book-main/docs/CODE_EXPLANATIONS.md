# Kod Açıklamaları

Bu doküman kodun her satırını ezberletmek için değil, önemli kararların neden alındığını anlatmak için hazırlanmıştır.

## HTML

- `<!doctype html>`: Tarayıcıya modern HTML standardını kullanacağını bildirir.
- `<html lang="tr">`: Sayfanın dilini belirtir; ekran okuyucu ve arama motorları için faydalıdır.
- `meta viewport`: Mobil cihazlarda sayfanın gerçek cihaz genişliğine göre ölçeklenmesini sağlar.
- `meta description`: Sayfanın içeriğini özetler.
- `header`, `nav`, `main`, `section`, `article`, `footer`: İçeriğin amacını ifade eden semantik etiketlerdir.
- `a href`: Başka bir sayfaya veya sayfa içindeki bir bölüme geçiş sağlar.
- `label for` ve `input id`: Etiket ile form alanını ilişkilendirir.
- `required`, `type="email"`, `minlength`: Tarayıcının temel form doğrulamasına yardım eder.
- `aria-label`: Görsel metni yeterli olmayan bir kontrolün amacını erişilebilir isimle belirtir.
- `aria-hidden="true"`: Yardımcı teknolojiye dekoratif içeriği yok saymasını söyler.
- `class`: CSS ile tekrar kullanılabilir stilleri ilişkilendirir.

## CSS mimarisi

- `base/reset.css`: Tarayıcıların varsayılan stillerinden kaynaklanan tutarsızlıkları azaltır.
- `base/variables.css`: Renk, font ve ölçüleri merkezi olarak yönetir.
- `base/typography.css`: Metin görünümü ve ortak yardımcı sınıflar.
- `layout/`: Header, footer ve sayfa genişliği gibi ana düzen.
- `components/`: Buton ve ürün kartı gibi yeniden kullanılan parçalar.
- `pages/`: Belirli sayfa gruplarına ait düzenler.
- `main.css`: Diğer dosyaları sırayla içe aktarır.

## CSS özellikleri

- `box-sizing: border-box`: Genişlik hesabına padding ve border'ı dahil ederek ölçü yönetimini kolaylaştırır.
- `clamp(min, preferred, max)`: Bir değerin ekranla birlikte esnemesini, fakat belirli sınırlar içinde kalmasını sağlar.
- `min()`: Sabit bir üst sınır ile mevcut alanı karşılaştırarak uygun genişliği seçer.
- `repeat(4, minmax(0, 1fr))`: Grid'de eşit dört sütun oluşturur ve sütun içeriğinin gereksiz taşma yapmasını azaltır.
- `@media`: Belirli ekran koşullarında farklı kurallar uygulamak için kullanılır.
- `:hover`: İşaretçi üzerine geldiğinde görünümü değiştirir.
- `:focus-visible`: Klavye gibi odak temelli kullanımda görünür odak göstergesi sağlar.
- `::before`: HTML'e yeni içerik eklemeden dekoratif katman oluşturabilir.

## Öğrencinin görevi

Her başlık için koddan bir örnek göster ve şu soruları cevapla:
1. Bu kod ne yapıyor?
 HTML: `aria-label - required`
**Örnek Kod:**
httml
<nav class="main-nav" aria-label="Ana navigasyon">
<input id="catalog-search" type="search" placeholder="Kitap ara…" required />
Menünün amacını ekran okuyucuya seslendirir, arama kutusunun boş gönderilmesini engeller.
2. Burada kullanılmasaydı ne olurdu?  **Cevap: Görme engelli kullanıcılar menüyü ayırt edemezdi, form boşken submit edilebilirdi.
3. Bu çözümün alternatifi var mı?  **Cevap: aria-labelledby vermek veya doğrulamayı saf JavaScript ile yapmak.
4. Hangi durumda bu yaklaşım uygun olmaz? **Cevap: Ekranda görünür net bir metin başlığı varsa veya JavaScript ile çok karmaşık form kontrolleri gerekiyorsa.
*Örnek Kod:*
Css
:root {
  --color-paper: #f8f6ef;
  --color-ink: #242720;
}
Bu kod ne yapıyor? **Cevap: Renkleri tek bir merkezde değişken olarak tanımlar ve tüm projede tekrar kullanılmasını sağlar.
​Burada kullanılmasaydı ne olurdu? **Cevap: Tüm CSS dosyalarında renk kodları elle yazılırdı, tema güncellemesi ve koyu tema eklemek imkansızlaşırdı.
​Bu çözümün alternatifi var mı? **Cevap: Tailwind gibi hazır kütüphaneler.
​Hangi durumda bu yaklaşım uygun olmaz? **Cevap: Tek sayfalık, birkaç satırlık çok küçük ve basit projelerde gereksiz yük oluşturur.