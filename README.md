# How to Read RJPEG

```
fir = flir_image_extractor.FlirImageExtractor()

def load_rjpg(path_image):
    path_image = '1.JPG'
    os.path.isfile(path_image)
    data = fir.extract_thermal_image()
    return data

data = load_rjpg('1.jpg')
```
