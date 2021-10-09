# Kullanim
config.js'de uretmek istediginiz gorsel adedini degistirdikten sonra index.js dosyasini calistirin
```bash
node index.js
```

Gorseller uretildikten sonra addon.js dosyasini calistirip gorsellerin JSON bilgileri istediniz ozellikler dogrultusunda yeniden organize edilecekler.
```bash
node src/addon.js
```

Kod satirlari islemlerin adim adim anlasilabilir olmasi ve tekrardan kullanicinin rahatca duzenleyebilmesi icin dokumantasyon eklendi.

# Opsiyonlar
`addon.js` 16. satirda Rank tanimlamalari mevcuttur. Gerekli bilgilendirme ayrica kod uzerinde yapildi.
`addon.js` 30. satirda JSON dosyalarina DNA bilgisi ekleyip eklememeyi secebilirsiniz. Eklemek icin true, eklememek icin false

# Eklemeler
`src/main.js`
- Mevcut programda bulunan resim yuzdeleri degistirildi.
- Programa puan algilama eklendi. Cikma yuzdesinden sonra `!` anahtari ile puan tanimlamasi yapilabilir.


`utils/rarityData.js`
- Asset kullanim orani global olarak diger dosyalar ile paylasilabilir olarak degistirildi. (fonksiyon: `getrarity()`)

## Dikkat
`addon.js` dosyasi bir defa calistirildiginiz zaman tekrar calistirmanizi onermiyorum. Zaten duzenlenmis olan JSON dosyalarini tekrar duzenlemeye calisinca hata verebilir.
`addon.js` dosyasi, `index.js` dosyasi calistirildiktan sonra 1 kez kullanilabilir.

Hepsi bu kadar :)
