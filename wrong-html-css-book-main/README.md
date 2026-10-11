# KitapKöşesi — HTML & CSS Proje Laboratuvarı

Bu proje, öğrencinin HTML ve CSS'i yalnızca konu konu öğrenmek yerine gerçekçi bir ürün üzerinde adım adım uygulaması için hazırlanmıştır. Proje, **çok sayfalı bir online kitap mağazası arayüzüdür**. Portfolyo veya tek sayfalık basit bir site değildir.

> Bu aşamada JavaScript kullanılmıyor. Sepete ekle, filtrele, arama ve form gönderimi gibi etkileşimler sonraki JavaScript aşamasında geliştirilecek. Şimdilik doğru HTML yapısı, CSS düzeni, responsive tasarım ve erişilebilirlik hedefleniyor.

## Projede neler var?

- Birden fazla HTML sayfası: ana sayfa, katalog, kitap detayı, sepet taslağı, üyelik/giriş ve iletişim
- Ortak CSS mimarisi: reset, değişkenler, layout, bileşenler ve sayfa stilleri
- Profesyonel klasör düzeni
- Öğrenci görevleri, aşama kontrol listeleri ve bonus görevler
- Kod açıklamaları ve code review kontrol listesi
- Bilerek hata eklenmiş hata ayıklama laboratuvarı
- `solutions/` altında hataların cevapları ve açıklamaları
- README ve teslim/GitHub yönergeleri

## Başlangıç

1. ZIP'i çıkar.
2. `index.html` dosyasını tarayıcıda aç veya VS Code'da Live Server kullan.
3. Önce `docs/LEARNING_PATH.md` dosyasını oku.
4. Her aşamayı sırayla bitir. Görevleri tamamlamadan sonraki aşamaya geçme.
5. Kodunu GitHub'a aşama aşama commit et.

## Beklenen klasör yapısı

```text
kitap-kosesi/
├── index.html
├── pages/
├── assets/
│   ├── images/
│   └── icons/
├── css/
│   ├── base/
│   ├── layout/
│   ├── components/
│   └── pages/
├── docs/
├── exercises/
│   └── debugging/
├── solutions/
└── README.md
```

## Tasarım hedefi

- Sıcak, modern bir kitap mağazası
- Krem arka plan, koyu mürekkep rengi, mercan vurgu rengi
- Okunabilir tipografi ve dengeli boşluklar
- Mobil, tablet ve masaüstüne uyum
- Klavye ve ekran okuyucu kullanımını destekleyen semantik HTML

## Tamamlanma ölçütü

- [x] Tüm sayfalar arasında tutarlı gezinme var.
- [x] Hiçbir sayfada yatay taşma yok.
- [x] HTML semantik ve girintileme tutarlı.
- [x] CSS tekrarları azaltılmış, değişkenler kullanılmış.
- [x] Form alanlarında label ve uygun input türleri var.
- [x] Görseller için anlamlı `alt` metinleri var.
- [x] Hata ayıklama görevleri çözüldü ve çözümlerle karşılaştırıldı.
- [x] Öğrenci code review listesini doldurdu.
- [x] GitHub deposunda anlamlı commit geçmişi var.

## Önemli not

`exercises/debugging/` içindeki dosyalarda **bilerek bırakılmış hatalar** bulunur. Önce `solutions/` klasörüne bakmadan çözmeye çalış. Çözümler öğretmen/öz değerlendirme amacıyla ayrı tutulmuştur.

# KitapKöşesi

KitapKöşesi, kitap severler için tasarlanmış modern, sade ve erişilebilir bir online kitapçı arayüzü konseptidir. Bu proje, temiz HTML5 semantiği ve modüler CSS mimarisi standartlarına uygun olarak geliştirilmiştir.

## 📄 Proje Sayfaları

- **Ana Sayfa (`index.html`)**: Öne çıkan kitaplar, avantajlar bandı ve bülten kayıt alanı.
- **Kitaplar / Katalog (`pages/catalog.html`)**: Kategori ve sıralama filtreleriyle listelenen kitap koleksiyonu.
- **Kitap Detayı (`pages/book-detail.html`)**: Kitap künyesi, açıklaması, puanı ve sepete ekleme alanı.
- **Favorilerim (`pages/favorites.html`)**: Kullanıcının kaydettiği kitapların listelendiği sayfa taslağı.
- **Sepetim (`pages/cart.html`)**: Boş sepet durumu ve alışveriş adımları taslağı.
- **Hikâyemiz (`pages/about.html`)**: Projenin ortaya çıkış vizyonu ve içerik düzeni.
- **İletişim (`pages/contact.html`)**: Kullanıcı geri bildirim ve mesaj formu.
- **Giriş Yap (`pages/login.html`)**: Kullanıcı giriş arayüzü taslağı.

## 🚀 Çalıştırma

Projeyi yerel ortamda görüntülemek için:

1. Proje klasörünü **VS Code** ile açın.
2. `Live Server` eklentisini kullanarak kök dizindeki `index.html` dosyasına sağ tıklayıp **"Open with Live Server"** seçeneğini seçin.
3. Tarayıcıda `http://127.0.0.1:5500` adresinden sayfalar arası gezinmeyi test edin.

## ⚠️ Bilinen Sınırlamalar

- **Dinamik İşlevler:** Sepete ürün ekleme/çıkarma, favori listesini güncelleme, arama ve filtreleme gibi dinamik mantıklar henüz aktif değildir; bu işlevler bir sonraki JavaScript aşamasında entegre edilecektir.
- **Form Gönderimleri:** İletişim ve bülten formları arayüz düzeyindedir; bir backend sunucusuna veya API'ye bağlı değildir.