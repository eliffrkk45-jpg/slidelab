# Nasse Biology (v2)

11. sınıf Biyoloji "1.5. Duyu Reseptörleri ve Duyu Organları" slaytlarına göre hazırlanmış interaktif site.
Saf HTML/CSS/JS: derleme gerekmez, GitHub Pages'te doğrudan çalışır.

## Dosyalar (hepsi AYNI klasöre konmalı)
index.html, style.css, data.js, models3d.js, sims.js, games.js, app.js, firebase-config.js

## Yayınlama (GitHub Pages)
1. Dosyaları repo köküne yükle (mevcut eski dosyaları silip yerine koy).
2. Settings > Pages > Branch: main / root.
3. Birkaç dakika sonra https://KULLANICI.github.io/REPO/ açılır.
Yerelde denemek için VS Code "Live Server" kullan (3B modeller ve fontlar internet ister: three.js ve Google Fonts CDN).

## Firebase giriş (isteğe bağlı)
firebase-config.js içindeki değerleri doldur; Authentication > Google'ı aç, Firestore oluştur, yetkili alan adlarına github.io ekle.
Boş bırakırsan ilerleme (XP, rozet) cihazda saklanır.

## Ne değişti
- Bağlam temelli sorular yenilendi (18 senaryo, 2 bölümlü yazılı cevap, model cevap + tolerans).
- Beynin bölümleri kaldırıldı.
- 3B modeller: göz, kulak, burun, dil, deri, nöron, sinaps (tıkla-bilgi kartı, döndür, yakınlaştır, dokunmatik).
- Ayrı "Konu Anlatımı" bölümü (Maarif: Merak Et > Öğren > Bağ Kur > Becerini Dene) 11 konu.
- Slayt kapsamı: uyaran/reseptör sınıflandırma, duyu organı-reseptör tablosu, hayvan örnekleri, nöron yapısı,
  eşik değer, ya hep ya hiç, merdiven etkisi, uyartı sıklığı, zar potansiyeli, sinaps, seçici direnç, göz-kamera/kulak-mikrofon.
- 4 simülasyon (her birinde önce görev, sonra gözlem sorusu), 5 oyun, 40 soruluk soru bankası.

## İçerik düzenleme
Konular, sorular ve bağlam soruları data.js içindedir. Bağlam sorusu cevap anahtarı: parts[].a listesi
(normalize edilir; "kelime1+kelime2" yazımında ikisi de geçmelidir).
