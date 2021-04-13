---
title: "Discussions"
weight: 1
description : "Dicussions and help can be found on forums or our chat services."
---

Dicussions and help can be found on our Forums (coming soon), Telegram or Matrix. Other services we do not trust and/or not proven themselves good enough to be used for communication.

<!-- ## LibreWeb Forums -->

## Instant chat

### Matrix

[Matrix](https://matrix.org) is a decentralized, open standard and federated communication protocol. You could use the [web version](https://element.io/), or install one of the many [Matrix Desktop clients](https://matrix.org/clients/) on your computer. Or even host your own Matrix server (Synapse) and become part of the federation. Both of which are open-sourced. Messages can be end-to-end encrypted if desired.

[Join official Matrix room](https://matrix.to/#/#libreweb:melroy.org?via=melroy.org).

{{%expand "Show installation instructions for Matrix Desktop Client on Debian/Ubuntu/Linux Mint." %}}

#### How-to install Matrix Element Desktop

```sh
sudo apt install -y wget apt-transport-https
sudo wget -O /usr/share/keyrings/riot-im-archive-keyring.gpg https://packages.riot.im/debian/riot-im-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/riot-im-archive-keyring.gpg] https://packages.riot.im/debian/ default main" | sudo tee /etc/apt/sources.list.d/riot-im.list
sudo apt update
sudo apt install element-desktop
```

{{% /expand%}}

#### Matrix homeservers

Matrix is decentralized, this means that in addition to the official matrix.org server, you can also register an account on other homeservers.  
My homeserver URL is open for public registrations: `https://matrix.melroy.org`.

### Telegram

Telegram is a cross-platform messaging service, clients are open-source (server is proprietary). Also messages are not encrypted by default, secret chats are encrypted.

[Join the official Telegram group](https://t.me/libreweb).
