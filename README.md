# MedBrothers Numbers

Ekip üyelerinin efsanevi sözlerini numaralandırıp Instagram story formatında sunan basit bir web sitesi.

## Özellikler

- Instagram story tarzı tam ekran slide navigasyonu
- Otomatik ilerleme (4sn) ve progress bar
- Dokunmatik: sağa dokun = sonraki, sola dokun = önceki, basılı tut = duraklat
- Klavye: sağ/sol ok tuşları, space
- Kişi bazlı renk temaları
- Mobil uyumlu
- Saf HTML/CSS/JS, harici bağımlılığı yok (font hariç)

## Kullanım

`index.html` dosyasını tarayıcıda aç. Hepsi bu.

## Yeni söz ekleme

`index.html` içindeki `slides` dizisine yeni bir obje ekle:

```js
{ number: 6, quote: '"Yeni söz buraya"', person: 'isim', author: '@isim' }
```

Yeni bir kişi ekliyorsan CSS'te ilgili renk temasını da tanımla:

```css
.slide[data-person="isim"]::before { background: radial-gradient(...); }
.slide[data-person="isim"] .big-number { color: #renk; }
.slide[data-person="isim"] .author { background: #renk; color: #000; }
.slide[data-person="isim"]::after { background: linear-gradient(90deg, transparent, #renk, transparent); }
.slide[data-person="isim"] .label { color: #renk; }
```

## Kişiler ve Renkleri

| Kişi | Renk |
|------|------|
| @aho | Turuncu (`#f97316`) |
| @gokhan | Mor (`#a78bfa`) |
| @derviş | Pembe (`#ec4899`) |
