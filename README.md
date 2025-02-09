# Pactus-Mainnet-Node-Setup

```
curl --proto '=https' --tlsv1.2 -sSL https://github.com/pactus-project/pactus/releases/download/v1.7.1/pactus_downloader.sh | sh
```

```
cd pactus-cli_1.7.1
```

```
./pactus-daemon init -w ~/pactus --restore "mnemonic"
```

```
apt install screen
screen -S pac
./pactus-daemon start -w ~/pactus
```

CTRL AD
```
./pactus-wallet --path ~/pactus/wallets/default_wallet address balance wallet-adress
```

Balance Control
```
./pactus-wallet --path ~/pactus/wallets/default_wallet address balance Wallet-adress
```

Validator Stake
```
./pactus-wallet --path ~/pactus/wallets/default_wallet tx bond <Wallet-adress> <Validator-Adress>
```
