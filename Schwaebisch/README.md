# Installatio

Zerst amål a Schritt-für-Schritt Ålôetong, wia mr s zom Laufa brengt.

## 1) tesseract installiera

Des *tesseract* ischd a digitals Werkzeug, zom älle mögliche Schrifta zom digitalisiera. 

- Älle Betriebssystem: [https://tesseract-ocr.github.io/tessdoc/Downloads.html](https://tesseract-ocr.github.io/tessdoc/Downloads.html),
- Windows: [https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki), dert die Datei `tesseract-ocr-w64-setup-5.5.0.20241111.exe` installiera.
- Dr Pfad en die PATH Variabla ergänza:
  - Ålôetong auf Englisch: [https://docs.coro.net/featured/agent/install-tesseract-windows](https://docs.coro.net/featured/agent/install-tesseract-windows)
  - Ålôetong auf Oxford-Deutsch: [https://ironsoftware.com/de/csharp/ocr/blog/ocr-tools/install-tesseract](https://ironsoftware.com/de/csharp/ocr/blog/ocr-tools/install-tesseract).
  
## 2) Fraktur für tesseract nåchlada

Standardmäßig kommt *tesseract* mit Englisch ond Deutsch. Theoretisch kå mr bei dr Installatio scho s entsprechende Paket mit lada, aber vo Håd nåchlada ischd der sichere Weg.
![](https://github.com/christofschroth/GermanFrakturToWord/blob/main/Images/deu_frak.png)

- Auf [https://github.com/tesseract-ocr/tesseract/wiki/Data-Files/e56d1a761f05007b6744d98108696f8c733349d7](https://github.com/tesseract-ocr/tesseract/wiki/Data-Files/e56d1a761f05007b6744d98108696f8c733349d7) sprenga, dert `deu_frak.traineddata` ralada.
- De Datei `deu_frak.traineddata` en dr Ordner `C:\Program Files\Tesseract-OCR\tessdata` kopiera (Admin-Rechte naedig!).

## 3) Python Bibliotheka installiera

Des Notebook *1_Install_Packages_tesseract.ipynb* laofa lao. Des muaß mr bloß oemål macha ond lädt insgesamt 3 naedige Bibliotheka.

## 4) Frakturschrift omwandla

Des Notebook *2_digitalize_german_fraktur.ipynb* laofa lao. I han a enstprechende Beispieldatei mit abglegt. R erstellt a Word-Datei mit am gleicha Dateinåma en dem Ordner, mô dia Datei dren ischd.