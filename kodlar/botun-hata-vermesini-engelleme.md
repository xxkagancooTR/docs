# Botun Hata Vermesini Engelleme

## 1. Bölüm Kodu Yapıştırma

Main dosyamızı buluyoruz. Dosyanın en altına kodu yapıştırıyorusunuz.\


```javascript
process.on('uncaughtException', (error) => {
    console.error('Beklenmeyen bir hata meydana geldi: ', error);
    // Uygulamanızın düzgün bir şekilde kapatılmasını sağlayabilirsiniz
    // Bu, hatalı işlemin devam etmesini önler ve gerektiğinde günlüğe kaydedebilir.
  });
  
  process.on('unhandledRejection', (reason, promise) => {
    console.error('Yakalanmamış bir vaat reddedildi:', reason);
    // Uygulamanızın düzgün bir şekilde kapatılmasını sağlayabilirsiniz
    // Bu, vaatin işlemesini engeller ve gerektiğinde günlüğe kaydedebilir.
  });
```
