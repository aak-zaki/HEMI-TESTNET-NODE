## HEMI TESTNET NODE RUN PROJECT 
Hemi Testnet Node is one of the most exciting blockchain projects with a confirmed airdrop and $15M funding. A Node Airdrop is also available! If you’re interested, participate now. All details are in the repository—don’t miss out on this potential. Start running your node today and earn rewards!


## 🔶TESTNET PHASE🔶 ##

1️⃣ Hemi Incentived Testnet (Backed by Binance Labs)

2️⃣ Join and complete testnet task

3️⃣ Bridge seth/usdt/udsc and earn points

4️⃣ And complete Galxe tasks

Full tutorial guide about testnet has been uploaded on our 
telegram channel go check it out

Link -- https://t.me/CryptoVenturesinkannada/2205


## System Requirements


| Hardware | Minimum Requirement  |
| :-------- | :------- |
|CPU| 2 Cores |
|RAM| 	2 to 4GB  |
|Disk| 50 to 100 GB |
|Bandwidth| 10 MBit/s |


As you know, you need a VPS to run this node project, so make sure to set up a VPS first. You can purchase a VPS through various online providers.

I'll recommend Contabo, a reliable and cost-effective option for VPS. Make sure to check it out and get your VPS set up before starting!

CONTABO VPS: [CLICK HERE](https://my.contabo.com/account/login)

## NOW LET'S RUN THE NODE




## ✦ Update and Install jq

```bash
sudo apt-get update
```
```bash
sudo apt-get install -y jq
```

## ✦ Check the architecture of your VPS using the following command:

```bash
uname -m
```

This command will return the architecture type, such as:

1️⃣ x86_64 for 64-bit Intel/AMD systems

2️⃣ arm64 for 64-bit ARM systems

If you see x86_64, it means your VPS is running on the x86_64 architecture, so choose commands that match this architecture type.

## Download the Binary for Your Architecture

Download the appropriate version based on your system architecture.

## ✦ For x86_64 Architecture:

```bash
wget --quiet --show-progress https://github.com/hemilabs/heminetwork/releases/download/v0.10.0/heminetwork_v0.10.0_linux_amd64.tar.gz -O heminetwork_v0.10.0_linux_amd64.tar.gz
tar -xzf heminetwork_v0.10.0_linux_amd64.tar.gz
cd heminetwork_v0.10.0_linux_amd64
```

## ✦ For arm64 Architecture:

```bash
wget --quiet --show-progress https://github.com/hemilabs/heminetwork/releases/download/v0.10.0/heminetwork_v0.10.0_linux_arm64.tar.gz -O heminetwork_v0.10.0_linux_arm64.tar.gz
tar -xzf heminetwork_v0.10.0_linux_arm64.tar.gz
cd heminetwork_v0.10.0_linux_arm64
```

## ✦ Wallet create

```bash
./keygen -secp256k1 -json -net="testnet" > ~/popm-address.json
```

## ✦ View Private Key and address

```bash
cat ~/popm-address.json
```

## ✦ Public Key for faucet

```bash
cat ~/popm-address.json | jq -r '.pubkey_hash'
```

Request Faucet tokens in disocrd -- [CLICK HERE](https://discord.gg/hemixyz)

## ✦ Create a servive file

```bash
sudo tee /etc/systemd/system/hemid.service > /dev/null << EOF

[Unit]
Description=Hemi testnet pop tx Service
After=network.target

[Service]
WorkingDirectory=/root/heminetwork_v0.10.0_linux_amd64
ExecStart=/root/heminetwork_v0.10.0_linux_amd64/popmd
Environment="POPM_BTC_PRIVKEY= replace here with your privatkey "
Environment="POPM_STATIC_FEE=200"
Environment="POPM_BFG_URL=wss://testnet.rpc.hemi.network/v1/ws/public"
Restart=on-failure

[Install]
WantedBy=multi-user.target
EOF
```
## ✦ Edit the service file

```bash
sudo nano /etc/systemd/system/hemid.service
```
Ensure that the environment variable is set inside the file, like this:

Environment="POPM_BTC_PRIVKEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"

Now save File :

Save : Ctrl + o , hit enter exit : Ctrl + x

## ✦ Start Miner service

```bash
sudo systemctl daemon-reload
sudo systemctl enable hemid.service
sudo systemctl start hemid.service
```

## ✦ Check logs

```bash
sudo journalctl -u hemid.service -f -n 50
```
Check you PoP Keystones Mined -- [CLICK HERE](https://testnet.popstats.hemi.network/)

Copy your wallet address and paste it into the link above to check if your node is running correctly. The process might take some time, typically between 1 to 3 hours, so be sure to check again later.

Thank you for exploring our repository! I hope you found valuable information through Crypto Ventures. 

📌If you're new to our repository and channel, make sure to follow us on our platforms for more updates and insights.

➣TELEGRAM IN KANNADA -- [CLICK HERE](https://t.me/CryptoVenturesinkannada)

➣TELEGRAM IN HINDI -- [CLICK HERE](https://t.me/CryptoVenturesinhindi)

➣INSTAGRAM IN KANNADA -- [CLICK HERE](https://www.instagram.com/cryptoventures_in_kannada?utm_source=qr&igsh=MXRjY2x0Y2lsMmJicg==)

➣INSTAGRAM IN HINDI -- [CLICK HERE](https://www.instagram.com/cryptoventuresinhindi?utm_source=qr&igsh=MXc1ZXNtdzJ0ZzFubw==)

➣YOUTUBE -- [CLICK HERE](https://youtube.com/@cryptoventures7723?si=Ym2bBsdz6HiLQQ2_)

➣TWITTER -- [CLICK HERE](https://x.com/SHASHI522004)

------------------------------★★★----------------------------------





















