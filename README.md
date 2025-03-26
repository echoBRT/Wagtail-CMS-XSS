# Wagtail-6.4.1-CMS-XSS
Wagtail CMS 6.4.1 Stored XSS

# CMS Stored XSS Vulnerability PoC

## Overview

This repository demonstrates a **Stored XSS** vulnerability found in the Wagtail 6.4.1 CMS platform. A malicious JavaScript is embedded in a PDF file, and every time a user clicks on the PDF, an XSS popup appears.

## Steps to Reproduce

1. Upload a PDF document that contains a malicious script, like the one provided in this repository.
![Ekran görüntüsü 2025-03-26 025701](https://github.com/user-attachments/assets/dddb03c7-ec89-45ef-8b95-1f5ae3fcf521)
![Ekran görüntüsü 2025-03-26 025903](https://github.com/user-attachments/assets/c5ad6c89-f81e-4b17-bb35-6c593ab0beb5)


2. Access the CMS and locate the malicious PDF.
3. Click on the PDF link.
![Ekran görüntüsü 2025-03-26 034822](https://github.com/user-attachments/assets/262e3839-8528-4d49-bec8-2acdab27e762)


5. The malicious JavaScript will trigger and display an XSS popup every time the PDF is opened.
6. 
![Ekran görüntüsü 2025-03-26 030008](https://github.com/user-attachments/assets/5e7d575c-6539-4d9e-b621-7c7db96df7bd)

## PoC Code

![pdf içeriği](https://github.com/user-attachments/assets/86249edb-1fed-4d13-9508-7f65c8731caa)

