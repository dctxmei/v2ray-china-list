# v2ray-china-list

This project converts [felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list) into a domain name file usable by V2Ray.

此項目將 [felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list) 轉換爲 V2Ray 可用的域名文件。

## Download links

- china-list.dat: [https://github.com/dctxmei/v2ray-china-list/releases/latest/download/china-list.dat](https://github.com/dctxmei/domain-list-community/releases/latest/download/china-list.dat)
- china-list.dat.sha256sum: [https://github.com/dctxmei/v2ray-china-list/releases/latest/download/china-list.dat.sha256sum](https://github.com/v2fly/domain-list-community/releases/latest/download/china-list.dat.sha256sum)
- china-list.dat.xz: [https://github.com/dctxmei/v2ray-china-list/releases/latest/download/china-list.dat.xz](https://github.com/dctxmei/domain-list-community/releases/latest/download/china-list.dat.xz)
- china-list.dat.xz.sha256sum: [https://github.com/dctxmei/v2ray-china-list/releases/latest/download/china-list.dat.xz.sha256sum](https://github.com/v2fly/domain-list-community/releases/latest/download/china-list.dat.xz.sha256sum)

## Usage example

Available tags:
* accelerated-domains.china
* apple.china
* google.china

```json
{
    "routing": {
        "rules": [
            {
                "type": "field",
                "domain": [
                    "ext:china-list.dat:accelerated-domains.china",
                    "ext:china-list.dat:apple.china",
                    "ext:china-list.dat:google.china"
                ],
                "outboundTag": "proxy"
            }
        ]
    }
}
```

## Thanks

This project is modified on the basis of [v2fly/domain-list-community](https://github.com/v2fly/domain-list-community) .
