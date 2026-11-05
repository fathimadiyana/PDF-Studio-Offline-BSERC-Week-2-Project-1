# PDF-Studio-Offline-BSERC-Week-2-Project-1
Project 1
A local desktop PDF utility built with Python, Tkinter, PyMuPDF, pypdf and Pillow.
It does not upload documents or call paid APIs. Once dependencies are installed, it can be used offline.
Run on Windows
1. Install Python 3.10 or newer.
2. Extract this ZIP.
3. Open Command Prompt in this folder.
4. Run:
   py -m pip install -r requirements.txt
   py pdf_studio.py
Run on Linux / Ubuntu
1. Install Python 3 and Tk support (Ubuntu: sudo apt install python3-tk).
2. In this folder run:
   python3 -m pip install -r requirements.txt
   python3 pdf_studio.py
Included tools
Organise: merge, split into single-page files, reorder, rotate, delete, duplicate, extract, insert blank, crop.
Edit: add text/image, highlight, draw, rectangle shape, whiteout, permanent redaction, typed signature, fill interactive form fields.
Stamp: watermark, page numbers, header/footer, date stamp.
Convert: images to PDF, PDF to PNG images, PDF to text.
Finish: compression with before/after sizes, edit metadata, remove common metadata, compare extracted text.
Important limitations and safe use
- This is a functional first implementation, not a certified PDF/A or forensic redaction product.
- Redaction applies to the selected rectangular area on the current page. Always export a separate copy and verify the output before sharing.
- Whiteout is a visual cover and is NOT secure redaction.
- Form filling supports interactive AcroForm fields when the PDF exposes them.
- Compare currently compares extracted text, not pixel-level visual differences.
- Crop uses margins in PDF points. PDF editing tools that ask for coordinates use points from the page's top-left.
- Some PDFs with unusual encryption, signatures, XFA forms or complex vector content may not behave as expected.
- The PDF is never automatically overwritten. Use Save As to export your edited document.
Testing checklist
Try with harmless sample PDFs:
- Merge two files; split a multi-page PDF; reorder pages; rotate; delete; duplicate; extract; insert a blank page; crop.
- Add text, image, highlight, draw, rectangle, whiteout and redaction to a test copy.
- Test stamps, conversions, metadata and compression.
- Compare two PDFs with known text changes.
- Disconnect Wi-Fi and repeat local operations.
