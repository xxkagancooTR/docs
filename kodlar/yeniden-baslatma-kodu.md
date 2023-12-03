# Yeniden Başlatma Kodu

## 1. Bölüm Kod

Verilecek kodu kendinize göre ayarlıyabilirsiniz.&#x20;

{% hint style="info" %}
Kod Pterodactyl Panel İçin Ayarlanmıştır
{% endhint %}

```javascript
  const time = moment.duration(client.uptime).format('D [days], H [hours], m [minutes], s [seconds]');
    const channel = client.guilds.cache.get("SUNUCUID").channels.cache.get("KANALID")
    await channel.send(`Bot is Restarting! Uptime time is **${time}**!`)
    await  exec('node bot.js', (error, stdout, stderr) => { //Main dosyanızı ayarlayın!
        if (error) {
          console.error(`Komut çalıştırma hatası: ${error}`);
          return;
        }
        console.log(`stdout: ${stdout}`); 
        console.error(`stderr: ${stderr}`);
      });
    
    // Yeni bir Node.js süreci başlatma
     await process.exit(0)
```
