# LoL Quiz

League of Legends temalı, Türkçe/İngilizce, mobil uyumlu mini quiz sitesi.

## Dosyalar
- `index.html`: sayfa yapısı
- `style.css`: tasarım ve mobil uyum
- `script.js`: dil, sorular, oyun mantığı, süre, skor ve yerel liderlik tablosu

## Bilgisayarında deneme
`index.html` dosyasına çift tıklayarak tarayıcıda açabilirsin. Daha sağlıklı test için VS Code içindeki Live Server eklentisini de kullanabilirsin.

## Ücretsiz GitHub Pages yayını
1. https://github.com adresinde ücretsiz hesap aç veya giriş yap.
2. Sağ üstte `+` → `New repository` seç.
3. Repository adı olarak `lol-quiz` yaz. `Public` seç ve `Create repository` düğmesine bas.
4. `Add file` → `Upload files` seç.
5. Bu klasördeki `index.html`, `style.css`, `script.js` dosyalarını sürükleyip bırak. (ZIP dosyasını değil, ZIP içindeki üç dosyayı yükle.)
6. `Commit changes` düğmesine bas.
7. Repository içinde `Settings` → sol menü `Pages` bölümüne gir.
8. `Build and deployment` altında `Deploy from a branch` seç.
9. Branch olarak `main`, klasör olarak `/ (root)` seç ve `Save` düğmesine bas.
10. Birkaç dakika sonra Pages ekranında `https://KULLANICI-ADIN.github.io/lol-quiz/` benzeri adresin görünür. Site adresin budur.

## İçerik düzenleme
- Sorular `script.js` dosyasının başındaki `bank` nesnesinde.
- Her soru için `q.tr` ve `q.en`, `o.tr` ve `o.en`, `a` (0'dan başlayan doğru seçenek) ve `why.tr` / `why.en` alanlarını düzenle.
- Eşya ve yetenek modlarındaki simgeler şu an prototip amaçlı sembollerdir; gerçek oyun ikonları değildir. Gerçek ikon eklemek için ilgili soruya `image` alanı ekleyip `renderQuestion()` içinde görseli gösterecek şekilde geliştirme yapılabilir.
- Puanlar ve rekor tablosu `localStorage` üzerinde, yani sadece aynı tarayıcı/cihazda tutulur. Ortak çevrimiçi sıralama için daha sonra veritabanı ve kullanıcı sistemi gerekir.

## Önemli not
Bu bağımsız bir hayran projesidir; Riot Games tarafından desteklenmez veya onaylanmaz. League of Legends, Riot Games'in ticari markasıdır. Riot'un oyun görsellerini, logolarını veya varlıklarını kullanmadan önce ilgili kullanım şartlarını ve fikri mülkiyet kurallarını kontrol et. Bu ilk prototipte özgün CSS tasarımı ve semboller kullanılmıştır.
