<h1 align="center"> Manta Network </h1>

![image](https://user-images.githubusercontent.com/101149671/195413725-5104a7f2-83b9-4c41-ad42-f91c51abbb0d.png)

## Sistem gereksinimleri:
```
Nefes alsın yeter
```



## Scirpt kurulumu (Hata alan olursa manuel kurulum aşağıda)

 * Ekip duyurusu: Katılan herkes için özel bir NFT almaya ve resmi Discord Kanalımızda özel bir unvan almaya hak kazanırsınız
 * Discord [linki](https://discord.gg/QTp6VhYm)

```
curl --proto '=https' --tlsv1.2 -sSf https://raw.githubusercontent.com/Manta-Network/manta-rs/main/tools/install.sh | sh
```

```
source ~/.profile
```

## Kurulum tamamlandıktan sonra twitter ve mail adresimizi giriyoruz ve çıktıyı kaydediyoruz



![image](https://user-images.githubusercontent.com/101149671/195415190-9f6e8b27-3269-4f19-8c2f-710a1b7e7524.png)


##  Çıktıyı aldıktan sonra form dolduruyoruz: [Link](https://mantanetwork.typeform.com/TrustedSetup)

 * Sunucuda girdiğimiz ve çıktıda verilen bilgilerle birebir aynı olmalı
 * Formda KMA adresi isteyecek, polkadot cüzdanı sağ üstte ayarlardan seçiyoruz calamari adresini
 * contribute daha açılmadı açıldığında 2 flood olarak paylaşırım.

![image](https://user-images.githubusercontent.com/101149671/195416025-6596a911-f12d-4ca1-9830-0ed33620f11b.png)


## Manuel:
```
sudo apt update
```

```
sudo apt install pkg-config build-essential libssl-dev curl jq
```

```
curl https://sh.rustup.rs/ -sSf | sh -s -- -y
```

```
source $HOME/.cargo/env
```

```
git clone https://github.com/Manta-Network/manta-rs.git
```

```
cd manta-rs
```

```
cargo run --release --package manta-trusted-setup --all-features --bin groth16_phase2_client register
```




