# Ehliyet Sınav Soruları — Gizlilik Politikası

Bu repo **Ehliyet Sınav Soruları** iOS/Android uygulamasının mağaza künyesine
verilen herkese açık sayfalarını barındırır. App Store Connect ve Google Play,
künyede gizlilik politikası ve destek için herkese açık adresler istediği için var.

Yayınlanan adresler:

- Gizlilik politikası: <https://berkegozukara.github.io/ehliyet-gizlilik/>
- Hesap silme talebi: <https://berkegozukara.github.io/ehliyet-gizlilik/hesap-silme/>
- Destek: <https://berkegozukara.github.io/ehliyet-gizlilik/destek/>

## Sayfalar elle düzenlenmez

Sayfalar, ana uygulama deposundaki `src/data/gizlilik-metni.ts` ve
`scripts/gizlilik-html.ts` dosyalarından üretiliyor — uygulama içindeki Ayarlar › Gizlilik Politikası ekranı da aynı
kaynaktan besleniyor. Metin değiştiğinde orada güncelleyip:

```
npm run gizlilik:html
```

çalıştırın. Çıkan dosyaları aşağıdaki hedeflere kopyalayıp commit'leyin:

- `docs/gizlilik.html` → `index.html`
- `docs/hesap-silme.html` → `hesap-silme/index.html`
- `docs/destek.html` → `destek/index.html`

Burada elle yapılan düzenleme bir sonraki üretimde kaybolur ve mağazadaki metin
uygulamanınkinden sapar.
