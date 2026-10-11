# Öğrenme Yol Haritası — HTML/CSS'ten JavaScript'e

## Proje kuralı

Bir aşamanın “bitti” sayılması için sadece sayfanın ekranda görünmesi yeterli değildir. Öğrenci yaptığı seçimi açıklayabilmeli, küçük değişiklikleri kendi başına yapabilmeli ve sayfayı farklı ekranlarda test etmelidir.

## Aşama 0 — Projeyi tanı ve ortamı hazırla
**Kavramlar:** klasör/dosya, göreli dosya yolu, tarayıcı, geliştirici araçları, Live Server.

Görevler:
- [ ] Projeyi bilgisayarına çıkar ve VS Code'da aç.
- [ ] `index.html` dosyasını Live Server ile çalıştır.
- [ ] `README.md` dosyasını oku.
- [ ] `css/main.css` içindeki her `@import` satırının hangi dosyayı bağladığını bul.
- [ ] Tarayıcıda bir bağlantıya tıkla ve adres çubuğunun nasıl değiştiğini gözlemle.

**Kontrol sorusu:** `pages/catalog.html` içinden ana CSS dosyasına neden `../css/main.css` yazılır?

## Aşama 1 — HTML belgesi ve semantik yapı
**Kavramlar:** `doctype`, `html`, `head`, `body`, başlık hiyerarşisi, `header`, `nav`, `main`, `section`, `article`, `footer`, bağlantı, liste.

Görevler:
- [ ] Ana sayfanın iskeletini kâğıda veya README'ye blok diyagram olarak çiz.
- [ ] Ana sayfadaki her `section` bölümünün amacını tek cümleyle açıkla.
- [ ] Katalog sayfasına yeni bir “Çok Satanlar” bölümü ekle.
- [ ] Her sayfada yalnızca bir ana `main` alanı olduğundan emin ol.
- [ ] Başlıkları sırayla kullan; sırf görünüş için başlık seviyesi atlama.

**Teslim:** HTML semantik kontrolü için ekran görüntüsü + commit.

## Aşama 2 — Metin, bağlantılar, listeler ve erişilebilirlik
**Kavramlar:** anlamlı bağlantı metni, `alt`, `aria-label`, `label`, skip link, klavye odağı.

Görevler:
- [ ] Tüm sayfaları bağlantılar üzerinden gez; kırık bağlantı bırakma.
- [ ] Bir navigasyon bağlantısının neden `aria-label` kullandığını açıkla. * Cevap: Ekran okuyucu kullanan görme engelli kullanıcılara menünün işlevini seslendirmek için kullanılır.
- [ ] `Tab` tuşuyla sayfada dolaş ve odak sırasını test et.
- [ ] Dekoratif öğelerde `aria-hidden="true"` kullanımını incele.
- [ ] Görsel eklersen anlamlı `alt` metni yaz; dekoratif görsel için boş alt kullanmanın ne zaman uygun olduğunu araştır. 

**Kontrol:** Bağlantı metinleri “buraya tıkla” gibi bağlamsız ifadeler olmamalı.

## Aşama 3 — Formlar ve HTML doğrulama
**Kavramlar:** `form`, `label`, `input`, `textarea`, `select`, `required`, `type=email`, `name`, `autocomplete`.

Görevler:
- [x] İletişim formuna telefon alanı ekle (`type="tel"`).
- [x] Telefon alanının zorunlu olup olmayacağına karar ver ve gerekçelendir.
- [x] E-posta alanına hatalı bir değer girerek tarayıcının yerleşik doğrulamasını test et.
- [x] Formdaki her `label` ile input `id` değerinin eşleştiğini kontrol et.
- [x] `name` niteliği olmayan bir input'un gönderim verisindeki farkını araştır.

**Not:** Formlar sunucuya bağlı olmadığı için gerçek mesaj gönderilmez.

## Aşama 4 — CSS temelleri ve cascade
**Kavramlar:** selector, specificity, inheritance, box model, margin, padding, border, renk, yazı tipi, pseudo-class.

Görevler:
- [x] `variables.css` içindeki `--color-coral` değerini değiştir ve tüm sitede nelerin etkilendiğini yaz. *Cevap: color-coral değişkeni değiştirildiğinde; tüm a butonlar (Sepetim, Bana Ulaşın, Mesajı Gönder, Kitapları Keşfet), sol üstteki logo amblemi ve vurgusu (`brand-mark`, `brand-accent`), başlıklardaki vurgu kelimeleri (italik yazılar), ana sayfadaki "Bizim Hikâyemiz" büyük banner bloğu ve mercan renkli kitap kapakları tek noktadan otomatik olarak yeni renge güncellendi.
- [x] Bir kartın iç boşluğunu `padding` ile, dış boşluğunu `margin` ile değiştir; farkı ekran görüntüsüyle göster.
- [x] `:hover` ve `:focus-visible` farkını açıkla.    *Cevap:hover, fareyle bir butonun veya linkin üstüne gelince çalışıyor. 
   focus-visible` ise klavyeden Tab tuşuyla gezerken hangi elemanda olduğumuzu görmemizi sağlıyor. Fareyle tıklayınca etrafında gereksiz kutu/çerçeve çıkarmıyor ama klavyeyle gezenler için odak çizgisini gösteriyor.
- [x] `content-pages.css` içine yeni selector eklemeden önce mevcut stilleri bul.    *Cevap:Yeni bir stil yazmadan önce `content-pages.css` dosyasına baktım.  önceden tanımlanmış sayfa başlığı, form ve grid stilleri olduğu için boş yere yeni seçici açıp kod tekrarı yapmadım, mevcut sınıfları kullandım.
- [x] Tarayıcı DevTools'ta bir elementin computed styles panelini incele. 

## Aşama 5 — Flexbox ve ortak bileşenler
**Kavramlar:** `display:flex`, `align-items`, `justify-content`, `gap`, flex-wrap, tekrar kullanılabilir sınıflar.

Görevler:
- [ ] Header içindeki marka, navigasyon ve aksiyon alanlarının hizalanmasını incele.
- [ ] Footer bağlantılarının neden dikey flex düzeni kullandığını açıkla.
- [ ] Bir buton varyantı oluştur: `.button-outline`.
- [ ] Butonun hover hâlini klavye odağıyla karıştırmadan test et.

## Aşama 6 — CSS Grid ve ürün kartları
**Kavramlar:** `display:grid`, `grid-template-columns`, `minmax`, `repeat`, responsive kart dizilimi.

Görevler:
- [ ] Kataloğa iki yeni kitap kartı ekle.
- [ ] Kartların farklı metin uzunluklarında nasıl davrandığını kontrol et.
- [ ] 4 sütundan 2 sütuna geçiş yapan media query'yi açıklayarak yorum satırı ekle.
- [ ] Grid'de `minmax(0, 1fr)` kullanımının taşmayı nasıl etkilediğini araştır.

## Aşama 7 — Responsive tasarım
**Kavramlar:** viewport, mobile-first düşünme, media query, `clamp`, esnek ölçüler, taşma testi.

Görevler:
- [ ] 1440px, 1024px, 768px, 390px ve 320px genişliklerde test et.
- [ ] Hiçbir ekran boyutunda yatay kaydırma olmamasını sağla.
- [ ] Bir mobil ekran görüntüsü ve bir masaüstü ekran görüntüsü teslim et.
- [ ] Media query'leri yalnızca gerektiği yerde ekle; her elemana ayrı breakpoint yazma.
- [ ] Dokunma hedeflerinin rahat kullanılabildiğini kontrol et.

## Aşama 8 — Tasarım sistemini anlama ve refactor
**Kavramlar:** CSS variables, ortak layout, naming, tekrar azaltma, dosya sorumlulukları.

Görevler:
- [ ] En az üç tekrar eden değeri CSS değişkenine dönüştür.
- [ ] Aynı işi yapan tekrar selector'ları bul ve birleştir.
- [ ] Yeni bir “favoriler” sayfasının iskeletini ortak header/footer yapısını kullanarak oluştur.
- [ ] Dosya adlarının ve sınıf adlarının amacını açıklayan mini sözlük yaz.

## Aşama 9 — HTML/CSS final kontrolü
- [ ] Tüm sayfalar birbirine bağlanıyor.
- [ ] Responsive kontroller tamamlandı.
- [ ] HTML doğrulayıcı ile hatalar kontrol edildi.
- [ ] CSS'te kullanılmayan kurallar temizlendi.
- [ ] Erişilebilirlik ve klavye odağı kontrol edildi.
- [ ] README'ye proje açıklaması, sayfalar, çalıştırma ve bilinen sınırlamalar eklendi.
- [ ] Code review checklist tamamlandı.

## JavaScript'e geçiş kapısı

Öğrenci aşağıdaki sorulara kendi cümleleriyle cevap verebiliyorsa JavaScript aşamasına geçebilir:
1. HTML ile CSS'in sorumlulukları nedir?
2. Semantik HTML neden önemlidir?
3. Flexbox ve Grid'i hangi durumda seçersin?
4. CSS cascade ve specificity bir çakışmayı nasıl çözer?
5. Responsive tasarım nasıl test edilir?
6. Bir formun tarayıcı doğrulaması ile sunucu tarafı doğrulaması arasındaki fark nedir?
7. Statik bir arayüzün neden tek başına sepet veya filtreleme yapamayacağını açıklayabilir misin?

**Sonraki modül:** JavaScript ile katalog arama/filtreleme, favorilere ekleme, sepet adedi ve toplam tutarı hesaplama, form geri bildirimi. Ardından modüler JavaScript ve daha sonra React bileşenlerine geçiş.
