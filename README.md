# ipfs-doc

Tìm hiểu về IPFS

## IPFS

Add 1 folder lên

```
cd <folder>
ipfs add -r .
```

## IPNS

Xử lý khi update content => Địa chỉ của 1 resource thay đổi

```
ipfs name publish /ipfs/QmaMLRsvmDRCezZe2iebcKWtEzKNjBaQfwcu7mcpdm8eY2
ipfs key gen SecondKey
ipfs name publish --key=SecondKey /ipfs/QmUVTKsrYJpaxUT7dr9FpKq6AoKHhEM7eG1ZHGL56haKLG
```

## DNSLink

DNSLink is currently much faster than IPNS and also uses human-readable names
DNSLink uses DNS TXT records (opens new window)to map a DNS name, like ipfs.io, to an IPFS address.

Update DNS config

```
dig +noall +answer TXT \_dnslink.docs.ipfs.io
> \_dnslink.docs.ipfs.io. 30 IN TXT "dnslink=/ipfs/bafybeieenxnjdjm7vbr5zdwemaun4sw4iy7h4imlvvl433q6gzjg6awdpq"
```

More detail (https://dnslink.dev/)[dnslink.dev]
