<h1 align="center"> Dymension Rollapp
  
![image](https://pbs.twimg.com/profile_banners/1506297383793176584/1685363195/1500x500)

## Sistem gereksinimleri:
### Ubunutu 22.04
NODE TİPİ | CPU     | RAM      | SSD     |
| ------------- | ------------- | ------------- | -------- |
| Dymension Rollapp  | 4         | 8         | 160  |
  

# Node Güncelleyelim

```
sudo apt-get update -y && sudo apt-get upgrade -y
```
### Gerekli Kütüphaneleri indiriyoruz.
```
sudo apt install curl tar wget clang pkg-config libssl-dev jq build-essential bsdmainutils git make ncdu gcc git jq chrony liblz4-tool -y
```
```
curl -L https://dymensionxyz.github.io/roller/install.sh | bash
```

![Ekran görüntüsü 2024-02-04 011820](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/12ab42c9-ebde-4950-84c8-52f6d5e6ec3a)

* Roller versiyon kontrolü;

```
roller version
```

![Ekran görüntüsü 2024-02-04 011941](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/e8da0fe2-b378-4ac4-a5b6-6a7e77e86e79)


### Rollap için gerekli ayarlamalrı yapıyoruz.
```
roller config init --interactive
```
![Ekran görüntüsü 2024-02-04 012054](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/04bdf7ca-2a1b-4551-aeab-2b54d23f2cdc)

* Froopyland ağını seçiyoruz.

![Ekran görüntüsü 2024-02-04 012139](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/9b16ca44-50d1-482a-955f-01493e2042e4)

* EVM Rollapp'i seçiyoruz.

![Ekran görüntüsü 2024-02-04 012404](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/c745df05-521a-456d-888a-36131fd96b65)

* Kendi Rollapp'inize verdiğiniz ismi yazın. Özel karakterler ve büyük harf kullanmayın! (-,* " gibi.)

![Ekran görüntüsü 2024-02-04 012506](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/53d82d34-4a32-4e3d-841c-bfd9e31d3dab)

* Token sembolünü seçiyoruz ETH, BTC gibi büyük harfle semboller girin. (Türkçe karakter kullanmayın.)

![Ekran görüntüsü 2024-02-04 012621](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/56dc6dfc-9005-43fb-8673-903895e7eed4)

* Token adedini belirliyoruz. Rastgele gelen miktar 1 Milyar adet daha fazla istiyorsanız sonuna sıfır ekleyebilirsiniz.

# Dikkat Komutu Girmeden önce alttaki görselleri ve açıklamaları okuyun.

* Komutu başlatınca ilk olarak sizden bir chain ismi isteyecek. İstediğiniz bir ismi girebilirsiniz.

![Ekran görüntüsü 2024-01-25 232028](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/855de031-ad14-46b7-88bc-011333f8765f)

* İkinci adımdaki seçimi ENTER yapıp geçiyoruz.

![Ekran görüntüsü 2024-01-25 232058](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/5de29fce-115c-42cf-a055-fcb30d827486)

* Üçüncü adımda Çalıştıracağımız DA seçiyoruz. Burada AVAIL seçimi yapacağız.

![Ekran görüntüsü 2024-01-25 232115](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/ae813da1-c25c-4181-bda3-515043599c32)

# ÇOK ÖNEMLİ!
![Ekran görüntüsü 2024-02-04 012747](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/4e2f0428-b785-47d9-8205-d630eafe0635)

* Burada seçimi AVAIL'i seçiyoruz.
## Yukarıdaki adımları doğru şekilde tamamlarsanız aşağıdakine benzer bir çıktı alacaksınız.

![Ekran görüntüsü 2024-02-04 012901](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/5fdd05b2-4a2e-48e8-ac6e-29fb140f5d62)

* Burada size verilen DYM adreslerine Dymension discordundan DYM test tokeni istiyorsunuz. Dymension discorduna katılmadıysanız [BURADAN](https://discord.gg/dymension) katılabilirsiniz. Faucet kanallarına ulaşmak için #intro-lounge kanalında kendiniz hakkında bir şeyler yazın discorda giriş yapabilirsiniz. (Daha önce katıldıysanız zaten faucetlere ulaşabiliyorsunuz. Her iki DYM adresine de faucet isteyin.)

## Devam etmeden önce OKU!!

* ilk defa AVAIL'e katılyorsan ve daha önce AVAIL'den token istemediysen senlik bir durum yok, Aşağıda senin için not bırakacağım oradan devam et.
* Madara yada daha önce AVAIL testine katılıp puan aldığın cüzdanı eklemek istiyorsan aşağıdaki adımları yap!

```
nano /root/.roller/da-light-node/avail.toml
```


# Not: BURADA size yeni bir AVAIL adresi verecek onu AVAIL'de puan kastığımız cüzdan ile değiştireceğiz.

# Not-2: Eğer ilk defa katılacaksanız. Aşağıdaki komutu çalıştırıp içindeki bilgileri bir yere not edin. Devam etmeden önce AVAIL discordundan [BURADAN](https://discord.gg/availproject) giriyoruz. Gitcoin pass puanımızın 20 ve üzerinde olması gerekiyor. Discord ve Gitcoin Pass doğrulamasını yaptıktan sonra Goldberg Faucet kanalından node içinde oluşan cüzdana token istiyoruz. Tokenler geldikten sonra aşağıdaki işlemlere devam ediyoruz.


İlk olarak aşağıdaki komutu giriyoruz. "" dahil aradaki notu silip  app'e verdiğin isimle değiştiriyorsun.
```
nano /root/.madara/app-chains/"Verdiğin App name ismi"/da-config.json
```
![Ekran görüntüsü 2024-01-25 232340](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/88e2fd32-1109-4d78-8f1a-dce8902d44be)

* Benzer bir sayda açılacak "seed":"0x... yazan yerdeki private key silip Cüzdan kelimelerimizi ekliyoruz. Son bölümdeki cüzdan adresini de AVAIL'deki cüzdan adresiyle değiştiriyoruz.

* CTRL X Y ve ENTER basıyoruz.

### Gerekli Portları açıyoruz.
```
sudo ufw enable
sudo ufw allow 22
sudo ufw allow 4000
sudo ufw allow 5353
sudo ufw allow 47250
sudo ufw allow 39276
sudo ufw allow 36347
sudo ufw allow 43759
sudo ufw allow 40815
sudo ufw allow 30333
sudo ufw allow 9944
sudo ufw allow 9615
```
### Yeni bir screen açalım
```
sudo apt install screen
```
```
screen -S roller
```
### App-chaini çalıştırıyoruz.

```
./target/release/madara run
```
Çalıştıktan sonra bloklar akmaya başladığında CTRL A+D ile çıkıyoruz.

### Exlporer sayfamızı çalıştıralım
```
cd
cd madara-cli
./target/release/madara explorer --host=IPADRESIN
```
Bu çalıştıktan sonra. http://SUNUCUIPADRESI:4000 sayfasından app-chaininize ait explorer ulaşabilirsiniz.

![Ekran görüntüsü 2024-01-26 003113](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/b568b4b2-d4ab-4e9d-a2df-92c06fe9afb3)

### En son App yayınlayalım

Önce aşağıdaki örnek olan komutları uyarılara göre düzenliyoruz.
```
  {
    "name": "App Name",
    "logo": "https://imgur.com/c09XXKf.png", // profil fotosu yüklüyoruz.
    "rpc_url": "http://IPADRESIN:9944",
    "explorer_url": "http://IPADRESIN:4000",
    "metrics_endpoint": "http://IPADRESIN:9615/metrics", 
    "id": "812de564-4f60-4ea0-b35f-5e7143769fbc" // uid alıyoruz.
  }
```
* ID almak için [BURADAN](https://www.uuidgenerator.net/) siteye gidiyoruz. Refresh yapıyoruz. çıkan ID alıp kopyalıyoruz.

![Ekran görüntüsü 2024-01-27 215100](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/3f519de4-93c8-4167-8545-786729ba784c)

400x400 boyutunnda bir resim ayarlıyoruz. [BURADAN](https://resimlink.com/)

![Ekran görüntüsü 2024-01-27 215606](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/b336b64a-e32c-44b3-b8b3-e7b5d320fe18)

* Resim Direkt linki alıp Yukarıdaki json dosyanıza ekleyebilirsiniz.

* Yukarıdaki komutları düzenleyiyoruz. Bir tane json dosyası oluşturuyoruz. Dosya isminiz aldığınız ID ismi olacaktır.

![Ekran görüntüsü 2024-01-27 220406](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/67f0ebd0-44eb-4309-bae2-39fd9286dc37)


## PR Açıyoruz.

[BURADAN](https://github.com/karnotxyz/avail-campaign-listing) buraya gidiyoruz ve ilk olarak Forkluyoruz.

![Ekran görüntüsü 2024-01-27 215811](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/e75cae6d-b503-49ed-b73b-222a1ee56d1c)

Forkladıktan sonra app-chains klasörüne giriyoruz.

![Ekran görüntüsü 2024-01-27 215936](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/0437e175-a142-44c7-a465-d48ef194dd89)

* Buradan hazırladığımız json dosyasını buraya yüklüyoruz. 

![Ekran görüntüsü 2024-01-27 220708](https://github.com/CoinHuntersTR/Avail-Full-Node/assets/111747226/38efaa74-0a00-499a-93f7-5f66d3ff3853)

Yükledikten sonra sağ üstten Pull Request yapıyoruz. Başlık bölümüne ✨ Adding verdiğiniz app ismi şeklinde yazabilirsiniz.





