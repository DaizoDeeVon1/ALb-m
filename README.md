# Bizim Hikâyemiz 💌

Romantik, animasyonlu dijital anı defteri. Sadece HTML, CSS ve JavaScript — sunucu gerekmez.

## Dosyalar

| Dosya | Ne işe yarar |
|---|---|
| `index.html` | Sayfanın yapısı |
| `style.css` | Görünüm ve animasyonlar |
| `script.js` | Çalışma mantığı |
| `ayarlar.js` | **Senin düzenleyeceğin dosya:** tarih, albüm adları, fotoğraflar, mektuplar |
| `foto/` | Fotoğraflarını buraya koy |

## GitHub'da yayınlama (GitHub Pages)

1. GitHub'da **New repository** ile yeni bir depo aç (örn. `bizim-hikayemiz`).
2. **Add file → Upload files** ile bu klasördeki tüm dosyaları (`.nojekyll` dahil) sürükle bırak, **Commit changes**'e bas.
3. Depoda **Settings → Pages** bölümüne gir. **Source** olarak *Deploy from a branch*, branch olarak **main** ve klasör olarak **/(root)** seç, **Save**'e bas.
4. 1-2 dakika sonra sitenin adresi sayfanın üstünde görünür:
   `https://KULLANICI-ADIN.github.io/bizim-hikayemiz/`

## Fotoğraf ekleme

1. Depoda **Add file → Upload files** ile fotoğrafları `foto` klasörüne yükle.
   Dosya adlarında **Türkçe karakter, boşluk ve büyük harf kullanma** (`ilk-bulusma.jpg` gibi).
2. `ayarlar.js` dosyasını açıp ✏️ ile düzenle ve `PHOTOS` listesine ekle:
   ```js
   { file: 'foto/ilk-bulusma.jpg', album: 0, date: '12 Mart 2023', note: 'O gün çok güzeldi ❤️' },
   ```
3. **Commit changes** de, site 1-2 dakikada güncellenir.

Büyük fotoğrafları yüklemeden önce küçült (en fazla ~1600 piksel genişlik): site hızlı açılır.

## Yazıları sitenin üzerinden değiştirme

Sitede sol alttaki **✎ Düzenle** butonuna bas, yazıların üstüne tıklayıp değiştir.
Bu değişiklikler önce sadece senin tarayıcında görünür. Herkesin görmesi için:

1. Düzenle panelinde **⬇ ayarlar.js olarak indir** butonuna bas.
2. İnen `ayarlar.js` dosyasını GitHub'a yükleyip eskisinin üzerine yaz (Commit).
3. Kendi tarayıcındaki eski değişiklikleri temizlemek için panelde **Yazı ve ayarları sıfırla** butonuna bas.

> Not: Sitede eklediğin fotoğraflar ve kapak/hikâye resimleri yalnızca senin tarayıcında kalır.
> Herkesin görmesi için fotoğrafı `foto` klasörüne yükleyip `ayarlar.js`'e yaz
> (kapaklar için `albumCovers`, hikâye fotoğrafı için `storyPhoto`).

## Gizlilik ⚠️

GitHub Pages'te yayınlanan siteyi ve **depodaki fotoğrafları linki bilen herkes görebilir**
(public depoda herkes bulabilir). Daha özel olmasını istiyorsan depoyu **private** yap
(private depoda Pages için ücretli plan gerekir) ya da fotoğrafları paylaşmadan önce düşün.
Site arama motorlarında çıkmasın diye `noindex` işareti eklendi, ama bu bir şifre değildir.
