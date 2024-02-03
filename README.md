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
* Froopyland ağını seçiyoruz.

![Ekran görüntüsü 2024-02-04 012054](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/04bdf7ca-2a1b-4551-aeab-2b54d23f2cdc)

* EVM Rollapp'i seçiyoruz.

![Ekran görüntüsü 2024-02-04 012139](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/9b16ca44-50d1-482a-955f-01493e2042e4)

* Kendi Rollapp'inize verdiğiniz ismi yazın. Özel karakterler ve büyük harf kullanmayın! (-,* " gibi.)

![Ekran görüntüsü 2024-02-04 012404](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/c745df05-521a-456d-888a-36131fd96b65)

* Token sembolünü seçiyoruz ETH, BTC gibi büyük harfle semboller girin. (Türkçe karakter kullanmayın.)

![Ekran görüntüsü 2024-02-04 012506](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/53d82d34-4a32-4e3d-841c-bfd9e31d3dab)

* Token adedini belirliyoruz. Rastgele gelen miktar 1 Milyar adet daha fazla istiyorsanız sonuna sıfır ekleyebilirsiniz.

![Ekran görüntüsü 2024-02-04 012621](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/56dc6dfc-9005-43fb-8673-903895e7eed4)



# ÇOK ÖNEMLİ!

* Burada seçimi AVAIL'i seçiyoruz.

![Ekran görüntüsü 2024-02-04 012747](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/4e2f0428-b785-47d9-8205-d630eafe0635)


## Yukarıdaki adımları doğru şekilde tamamlarsanız aşağıdakine benzer bir çıktı alacaksınız.

![Ekran görüntüsü 2024-02-04 012901](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/5fdd05b2-4a2e-48e8-ac6e-29fb140f5d62)

* Burada size verilen DYM adreslerine Dymension discordundan DYM test tokeni istiyorsunuz. Dymension discorduna katılmadıysanız [BURADAN](https://discord.gg/dymension) katılabilirsiniz. Faucet kanallarına ulaşmak için #intro-lounge kanalında kendiniz hakkında bir şeyler yazın discorda giriş yapabilirsiniz. (Daha önce katıldıysanız zaten faucetlere ulaşabiliyorsunuz. Her iki DYM adresine de faucet isteyin.)

## Devam etmeden önce OKU!!

* ilk defa AVAIL'e katılyorsan ve daha önce AVAIL'den token istemediysen senlik bir durum yok, Aşağıda senin için not bırakacağım oradan devam et.
* Madara yada daha önce AVAIL testine katılıp puan aldığın cüzdanı eklemek istiyorsan aşağıdaki adımları yap!

```
nano /root/.roller/da-light-node/avail.toml
```
![Ekran görüntüsü 2024-02-04 013647](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/b3efd93f-860c-4470-9249-186ba3632069)

* Burada Mnemonic yazan yerde tırnak içindeki kelimeleri sil ve AVAIL cüzdanının kelimelerini gir. Kendi cüzdan kelimelerini girdikten sonra CTRL X yapıp Y basıp ENTER diyerek çıkıyoruz.

```
nano /root/.roller/rollapp/config/dymint.toml
```
![Ekran görüntüsü 2024-02-04 014259](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/fa02a18c-05b4-40be-a321-63693859454c)

* Ekran görüntüsünde işaretlediğim yerdeki kelimeleri silip kendi cüzdan kelimelerini ekliyorsun. Sonra, CTRL X yapıp Y basıp ENTER ile kayıt edip çıkıyorsun.

```
roller keys list
```
* Yukarıdaki komut ile adreslerimizi tekrar listeliyoruz. Kendi AVAIL adresimizi orada görüyorsak, işlemlere devam edebiliriz.
![Ekran görüntüsü 2024-02-04 014902](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/ae9335ad-7c19-4293-afb0-b6f03d9d0e92)


### Devam edelim.
* Hey ilk defa kuran sen :D buradan başlayıp devam edebilirsin.
  
```
roller tx register
```
![Ekran görüntüsü 2024-02-04 015631](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/382a053f-d72f-4ce0-9a42-957b6d020910)

* Bu şekilde çıktı aldıysanız. İşlemler tamam devam edelim.

### Yeni Bir Screen Açalım

```
sudo apt install screen
```
```
screen -S rollapp
```
```
roller run
```
![Ekran görüntüsü 2024-02-04 020014](https://github.com/CoinHuntersTR/Dymension-Rollapp/assets/111747226/cb382028-1f76-4684-8873-9e3296834b61)

* Bu komutu çalıştırdıktan sonra, rollapp'in çalışması için channel bulması gerekiyor bu bazen 1 saat bazen 1 gün sürebilir. Channel bulana kadar bekliyoruz. Channel bulduktan sonra aşağıdaki adımlara devam edeceğiz.

* Bulunduğunuz ekrandan çıkmak için CTRL A sonra da D yapıp çıkabilirsiniz.
  
* Tekrar aynı screen içine girmek istiyorsanız aşağıdaki komutu kullanabilrsin.
  
 ```
screen -r rollapp
``` 

### Protlarımızı açalım
```
sudo ufw allow 22
sudo ufw enable
sudo ufw allow 26657
sudo ufw allow 8545
sudo ufw allow 1317
``` 
