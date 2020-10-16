Downloading input images (sRGB)
```
wget -c --http-user=anonymous --http-password=anonymous -i WideGamutDataset_srgb-8bpc.txt -P ./WideGamutDataset/srgb-8bpc
```

Downloading target images (ProPhoto RGB)
```
wget -c --http-user=anonymous --http-password=anonymous -i WideGamutDataset_prop-8bpc.txt -P ./WideGamutDataset/prop-8bpc
```

Downloading split information
```
wget -c --http-user=anonymous --http-password=anonymous -i WideGamutDataset_split.txt -P ./WideGamutDataset/split
```