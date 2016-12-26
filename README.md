# jid_release_deb

[![build status](https://gitlab.com/bpicode/jid_release_deb/badges/master/build.svg)](https://gitlab.com/bpicode/jid_release_deb/commits/master)

[![Download](https://api.bintray.com/packages/bpicode/jid_deb/jid/images/download.svg)](https://bintray.com/bpicode/jid_deb/jid/_latestVersion)

This repository automates the building of debian packages for
[jid](https://github.com/simeji/jid), the JSON Incremental Digger.

## Install (debian/ubuntu/...)

Add the repository

```bash
echo "deb https://dl.bintray.com/bpicode/jid_deb jessie main" | sudo tee -a /etc/apt/sources.list
```

and its signing key

```bash
wget -qO - https://api.bintray.com/users/bpicode/keys/gpg/public.key | sudo apt-key add -
```

The fingerprint of the repository key `3072D/35E71039` is
`93AC 2A3D 418B 9C93 2986  6463 15FC CFC9 35E7 1039`.
Update your local repository data and install

```bash
sudo apt update
sudo apt install jid
```
