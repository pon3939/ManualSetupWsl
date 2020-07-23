# WSLセットアップ手順書

## インストール

「コントロール パネル -> プログラム -> プログラムと機能」で「Windows Subsystem for Lynux」を有効化して再起動

Microsft StoreでUbuntuをインストール

## 初期設定

Ubuntuを起動する

初回起動時にはユーザー名、パスワードを聞かれる。パスワードはsudoするときに必要。

パッケージを更新

```bash
sudo apt update
sudo apt upgrade -y
```

日本語化

```bash
sudo apt install -y language-pack-ja
sudo update-locale LANG=ja_JP.UTF-8
sudo dpkg-reconfigure tzdata
sudo apt install -y manpages-ja manpages-ja-dev
```

## その他

`\\wsl$`でWindowsからLinuxのファイルシステムにアクセスできる

`\mnt`でLinuxからWindowsのファイルシステムにアクセスできる