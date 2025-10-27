# Installation

Step-by-step manual.

## 1) Install tesseract

*Tesseract* is a digital tool to recognize different kind of written or printed letters. 

- All operation systems: [https://tesseract-ocr.github.io/tessdoc/Downloads.html](https://tesseract-ocr.github.io/tessdoc/Downloads.html),
- Windows: [https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki), download and install the file `tesseract-ocr-w64-setup-5.5.0.20241111.exe`.
- Add path to Windows Environment variables, see [https://docs.coro.net/featured/agent/install-tesseract-windows](https://docs.coro.net/featured/agent/install-tesseract-windows).
  
## 2) Upgrade fraktur for tesseract

Usually, the *fraktur* is not delivered with the standard installation of *tesseract*. Though it can be added during the installation, the safe way is to download it manually.
![](https://github.com/christofschroth/GermanFrakturToWord/blob/main/Images/deu_frak.png)

- ´Go to [https://github.com/tesseract-ocr/tesseract/wiki/Data-Files/e56d1a761f05007b6744d98108696f8c733349d7](https://github.com/tesseract-ocr/tesseract/wiki/Data-Files/e56d1a761f05007b6744d98108696f8c733349d7) and download the file `deu_frak.traineddata`.
- Copy the file `deu_frak.traineddata` to `C:\Program Files\Tesseract-OCR\tessdata` (Admin-rights required).


## 3) Install python libraries

Take the notebook *1_Install_Packages_tesseract.ipynb* and run. You need to do this once at the start, it will load and install 3 required libraries.

## 4) Transformation of fraktur

Run the notebook *2_digitalize_german_fraktur.ipynb*. In the folder *Images* you'll find the example file *deu_frak.png*. The notebook will produce a word file in the same folder where you provide the image.