# Durum Değiştirme

## 1. Bölüm Kod Dosyasını Bulma

Genellikle kodu atacağımız dosya ya **main** dosyanızdır. Yada ready.js dir.\
\


## 2. Bölüm Ready.JS ekleme

```javascript
    client.user.setPresence({
      activities: [{ name: `saganetwork.net`}],
      status: 'idle',
    });
```

Kodunu alıp ready.js dosyamıza yapıştırıyoruz.\
\


## 3. Bölüm Main.JS (BOT.JS) ekleme

```javascript
    client.on("ready", () => {
client.user.setPresence({
      activities: [{ name: `saganetwork.net`}],
      status: 'idle',
    });
})
```

Kodumuzu main dosyamıza yapıştırıyoruz.
