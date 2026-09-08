# PDF Image Extractor

A simple Windows desktop app for extracting images from PDF files.

The app uses Poppler's `pdfimages` tool to extract images directly from PDFs and saves them into separate folders for each PDF.

## Features

* Extract images from multiple PDFs at once
* Adjustable worker count for parallel processing

## How It Works

Select a folder containing PDF files.

For example:

```text
Stock/
├── document1.pdf
├── document2.pdf
└── document3.pdf
```

Choose an output folder and click **Extract Images**.

The app creates a separate folder for each PDF:

```text
Extract/
├── document1/
│   ├── image-000.png
│   ├── image-001.png
│   └── image-002.png
├── document2/
│   ├── image-000.png
│   └── image-001.png
└── document3/
    └── image-000.png
```

## Windows Download

Download the Windows build from the repository's Releases section or download the repository as a zip.

After downloading, extract the ZIP file and run:

```text
PDFImageExtractor.exe
```

## Troubleshooting

Make sure the pdfimages.exe and python.exe has controlled folder access in windows defender, check protection history to see if you are running into this issue
