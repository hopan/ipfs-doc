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

