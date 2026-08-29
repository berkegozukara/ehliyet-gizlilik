# Ehliyet Sınav Hazırlık — Gizlilik Politikası

Bu repo yalnızca **Ehliyet Sınav Hazırlık** iOS/Android uygulamasının gizlilik
politikasını barındırır. App Store Connect ve Google Play, mağaza künyesinde
herkese açık bir "Privacy Policy URL" istediği için var.

Yayınlanan adres: <https://berkegozukara.github.io/ehliyet-gizlilik/>

## index.html elle düzenlenmez

Sayfa, ana uygulama deposundaki `src/data/gizlilik-metni.ts` dosyasından
üretiliyor — uygulama içindeki Ayarlar › Gizlilik Politikası ekranı da aynı
kaynaktan besleniyor. Metin değiştiğinde orada güncelleyip:

```
npm run gizlilik:html
```

çalıştırın, çıkan `docs/gizlilik.html` dosyasını buraya `index.html` olarak
kopyalayıp commit'leyin. Burada elle yapılan düzenleme bir sonraki üretimde
kaybolur ve mağazadaki metin uygulamanınkinden sapar.
