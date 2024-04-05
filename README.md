# How to Read RJPEG

## How to install and use in macos

1. Go to https://exiftool.org/ URL
2. Download and install exiftool
3. locate path of exiftool binary
4. Assign path_exit_tool to it. Usually it is '/usr/local/bin/exiftool'

```
path_exit_tool = '/usr/local/bin/exiftool'

fir = flir_image_extractor.FlirImageExtractor(exiftool_path=path_exit_tool)

def load_rjpg(path_image):
    path_image = '1.JPG'
    os.path.isfile(path_image)
    data = fir.extract_thermal_image()
    return data

data = load_rjpg('1.jpg')
```
