Update v1.7.1


```
cd
wget https://github.com/pactus-project/pactus/releases/download/v1.7.1/pactus-cli_1.7.1_linux_amd64.tar.gz
tar -xvf pactus-cli_1.7.1_linux_amd64.tar.gz
screen -r pactus
```

Ardından CTRL+C ile durduralım
```
cd
cd pactus-cli_1.7.1
./pactus-daemon start -w ~/pactus
```



📌Services📌
```
cd
systemctl stop pactusd
wget https://github.com/pactus-project/pactus/releases/download/v1.7.1/pactus-cli_1.7.1_linux_amd64.tar.gz
tar -xvf pactus-cli_1.7.1_linux_amd64.tar.gz
cp -r pactus-cli_1.7.1/* pac/
systemctl restart pactusd
journalctl -u pactusd -fo cat
```
