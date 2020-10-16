### 1. Before going further, change your working directory to somewhere desirable place.

Below commands will make ```'./WideGamutDataset'```, ```'./WideGamutDataset/srgb-8bpc'```, ```'./WideGamutDataset/prop-8bpc'```, and ```'./WideGamutDataset/split'``` directories.

Then the corresponding contents will be downloaded into matching directories.

### 2. Downloading input images (sRGB)
```
wget -c --http-user=anonymous --http-password=anonymous -i WideGamutDataset_srgb-8bpc.txt -P ./WideGamutDataset/srgb-8bpc
```

### 3. Downloading target images (ProPhoto RGB)
```
wget -c --http-user=anonymous --http-password=anonymous -i WideGamutDataset_prop-8bpc.txt -P ./WideGamutDataset/prop-8bpc
```

### 4. Downloading split information.
```
wget -c --http-user=anonymous --http-password=anonymous -i WideGamutDataset_split.txt -P ./WideGamutDataset/split
```
After downloading split information, please replace paths in each file correctly. For example, change the content from
```
# Original 'WideGamutDataset/split/train-input.txt'
Z:\WideGamutDataset\srgb-8bpc\standard-nuscc-OlympusEPL6_0142.png
Z:\WideGamutDataset\srgb-8bpc\vivid-fivek-a1616-_DGW6356.png
Z:\WideGamutDataset\srgb-8bpc\standard-fivek-a1281-tc_DSC2356.png
...
```
to as follows:
```
# Updated 'WideGamutDataset/split/train-input.txt'
<to_correct_directory>\WideGamutDataset\srgb-8bpc\standard-nuscc-OlympusEPL6_0142.png
<to_correct_directory>\WideGamutDataset\srgb-8bpc\vivid-fivek-a1616-_DGW6356.png
<to_correct_directory>\WideGamutDataset\srgb-8bpc\standard-fivek-a1281-tc_DSC2356.png
...
```
