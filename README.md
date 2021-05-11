# Discord Voice Bot(s)

# Kurulum
* İlk olarak bilgisayarına [Node JS](https://nodejs.org/en/) indir.
* Daha sonra bilgisayarına (eğer yoksa) FFMPEG kurmalısın. [Buraya tıklayarak nasıl kuracağını öğrenebilirsin](https://github.com/thearkxd/discord-welcome-bots#ffmpeg-kurulum)
* Bu projeyi zip halinde indir.
* Herhangi bir klasöre zipi çıkart.
* Daha sonra `settings.json` dosyasının içindeki bilgileri doldur.
  * "tokens": [] içine istediğiniz kadar token girebilir, ve o kadar ses botu açabilirsiniz.
* Sonra klasörün içerisinde bir `powershell` ya da `cmd` penceresi aç.
* ```npm install``` yazarak tüm modülleri kur.
* Kurulum bittikten sonra ```npm start``` yaz ve botu başlat.

Tada 🎉. Artık ses botların hazır. Dilediğin gibi kullanabilirsin.

# FFMPEG Kurulum
* [Eğer bilgisayarınız Windows ise tıklayın.](https://www.wikihow.com.tr/Windows%27ta-FFMpeg-Nas%C4%B1l-Kurulur)
* Eğer bilgisayarınız MacOS ise;
  * Öncelikle [homebrew](https://brew.sh/index_tr) indirin.
  * Daha sonra;
  ```
  $ brew install ffmpeg
  ```
  * komutu ile FFMPEG'i kurun.
  
# Glitch kullananlar için;
Eğer Glitch kullanıyorsanız ve token'larınızı `.env` (environment) dosyasına girmeniz gerekiyorsa;
* Öncelikle `.env` dosyasında yeni bir veri oluşturup (TOKENS gibi) tüm token'larınızı **aralarında boşluk bırakarak** giriniz.
* Daha sonra main dosyasına gelin ve;
```js
const { tokens, channels, staffRoles, unregisterRoles, welcomeSound, staffSound } = require("./settings.json");
```
* kısmını;
```js
const { channels, staffRoles, unregisterRoles, welcomeSound, staffSound } = require("./settings.json");
const tokens = process.env.TOKENS.split(" ");
```
* olarak değiştirin

Bu kadar 🎉

# İletişim
* [Discord Sunucum](https://discord.gg/UEPcFtytcc)
* [Discord Profilim](https://discord.com/users/350976460313329665)
* Herhangi bir hata bulmanız durumunda ya da yardım isteyeceğiniz zaman buralardan bana ulaşabilirsiniz.

### NOT: Botta MIT lisansı bulunmaktadır. Bu botun dosyalarının benden habersiz paylaşılması/satılması durumunda gerekli işlemler yapılacaktır!
