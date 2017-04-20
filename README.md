# pytesseract
The pytesseract.py file is updated for the Python 3 where the user is getting Access Denied error. The pytesseract.py will work smoothly with tesseract-ocr also

# Steps to follow

1. Downlod Tesseract-OCR from https://github.com/tesseract-ocr/tesseract
2. Add the available tesseract.exe file to the folder
3. In pytesseract.py , for variable 'tesseract_cmd', change the value to tesseract.exe path
4. Sample Code
```
from PIL import Image
import pytesseract

image = Image.open(r'toast.png')

print (image)
text = pytesseract.image_to_string(image)
print(text)
```
