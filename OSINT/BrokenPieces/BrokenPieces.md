# Broken Pieces

> Oh no! I broke this framed image. Unless you can magically put it together, I’m in big trouble.
> Flag format: CTF{...}

The task is to concatenate the images together. The way that the images are numbered suggest there are 20 rows and columns.

```python
from PIL import Image
import pathlib

def get_concat_h(im1, im2):
    dst = Image.new('RGB', (im1.width + im2.width, im1.height))
    dst.paste(im1, (0, 0))
    dst.paste(im2, (im1.width, 0))
    return dst

def get_concat_v(im1, im2):
    dst = Image.new('RGB', (im1.width, im1.height + im2.height))
    dst.paste(im1, (0, 0))
    dst.paste(im2, (0, im1.height))
    return dst

rows = []
i = 0
for file in pathlib.Path("./pieces").iterdir():
    if i == 0:
        row = Image.open(file)
    else:
        img = Image.open(file)
        row = get_concat_h(row, img)
    if i == 19:
        rows.append(row)
        i = 0
    else:
        i += 1
    
result = rows[0]
for i in range(len(rows)):
    result = get_concat_v(result, rows[i])

result.save("result.png")
```
Code is adapted from [here](https://note.nkmk.me/en/python-pillow-concat-images/). Scan the QR code to get the flag.

The flag is `CTF{th@nk2_f0r_h3lping}`
