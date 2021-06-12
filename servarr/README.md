`libseccomp2` needs to be installed from Debian Backports as per [linuxserver.io](https://docs.linuxserver.io/faq#libseccomp):

```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 04EE7237B7D453EC 648ACFD622F3D138
echo "deb http://deb.debian.org/debian buster-backports main" | sudo tee -a /etc/apt/sources.list.d/buster-backports.list
sudo apt update
sudo apt install -t buster-backports libseccomp2
```

# Servarr

## Media Management

Add root folder `/multimedia/{Movies,Shows}`

## Indexers

Add Jackett with URL `http://jackett:9117/api/v2.0/indexers/all/results/torznab`

## Download Clients

Add Deluge with `deluge-vpn` host
Add Transmission with `transmission-vpn` host

Add remote path mapping `deluge-vpn:/downloads` -> `/deluge`
Add remote path mapping `transmission-vpn:/downloads` -> `/transmission`
