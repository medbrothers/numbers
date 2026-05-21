# CLAUDE.md

## Proje Özeti

MedBrothers Numbers - ekip üyelerinin sık kullandığı sözleri Instagram story formatında gösteren tek sayfalık statik site.

## Teknoloji

- Saf HTML + CSS + vanilla JS (tek dosya: `index.html`)
- Framework yok, build step yok
- Google Fonts (Space Grotesk + Outfit)

## Mimari

Her şey `index.html` içinde:
- CSS: style etiketi içinde
- JS: script etiketi içinde
- Slide verileri: `slides` dizisi (JS içinde)

## Önemli Notlar

- Yeni söz eklerken `slides` dizisine obje ekle ve progress bar otomatik güncellenir
- Yeni kişi eklerken CSS'te renk teması tanımlanmalı (`data-person` attribute ile eşleşir)
- Story süresi `STORY_DURATION` sabiti ile kontrol edilir (ms cinsinden, varsayılan: 4000)
- Site mobil-öncelikli tasarlanmıştır, dokunmatik etkileşim birincil navigasyondur
