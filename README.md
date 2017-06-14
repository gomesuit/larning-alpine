```
vagrant plugin install vagrant-alpine
vagrant up
vagrant ssh
```

- 参考
  - https://github.com/maier/vagrant-alpine


## パッケージの管理
```sh
apk info

# install
apk add openssh

# 検索
apk search -v
apk search i3

# アップデートなど
apk update
apk upgrade

# 例
apk add zsh vim tmux git sudo perl automake cmake build-base qt
```

## コミュニティのパッケージをインストール
```/etc/apk/repositories
http://dl-4.alpinelinux.org/alpine/v3.3/main
http://dl-4.alpinelinux.org/alpine/v3.3/community
http://dl-4.alpinelinux.org/alpine/edge/testing
```
`apk update`

## デーモンの管理
```bash
rc-status
# 起動
rc-service slim start
# サービス登録
rc-update add slim
```

## ユーザーの作成
```bash
adduser test
cd /home/test
sudo visudo
```

## ネットワーク設定
```/etc/network/interfaces
iface eth0 inet static
        address 192.168.1.150
        netmask 255.255.255.0
        gateway 192.168.1.1
```
