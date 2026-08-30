# Ehliyet Sınav Hazırlık — Gizlilik Politikası

Bu repo yalnızca **Ehliyet Sınav Hazırlık** iOS/Android uygulamasının gizlilik
politikasını barındırır. App Store Connect ve Google Play, mağaza künyesinde
herkese açık bir "Privacy Policy URL" istediği için var.

Yayınlanan adresler:

- Gizlilik politikası: <https://berkegozukara.github.io/ehliyet-gizlilik/>
- Hesap silme talebi: <https://berkegozukara.github.io/ehliyet-gizlilik/hesap-silme/>

## index.html elle düzenlenmez

Sayfa, ana uygulama deposundaki `src/data/gizlilik-metni.ts` dosyasından
üretiliyor — uygulama içindeki Ayarlar › Gizlilik Politikası ekranı da aynı
kaynaktan besleniyor. Metin değiştiğinde orada güncelleyip:

```
npm run gizlilik:html
```

çalıştırın. Çıkan dosyaları aşağıdaki hedeflere kopyalayıp commit'leyin:

- `docs/gizlilik.html` → `index.html`
- `docs/hesap-silme.html` → `hesap-silme/index.html`

Burada elle yapılan düzenleme bir sonraki üretimde kaybolur ve mağazadaki metin
uygulamanınkinden sapar.
