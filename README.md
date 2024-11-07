# PDF Splitter 📄✂️

This is a Python-based script that splits a PDF file into two parts at a specified page. The script allows users to input a PDF file and define a split point (page number) where the PDF will be divided. The two resulting PDFs are saved as separate files in the specified output directory.

## Table of Contents
- [Features](#features)
- [How It Works](#how-it-works)
- [Requirements](#requirements)


## Features

- Splits a PDF file into two parts based on a user-defined page number.
- Saves the two parts in a specified output directory.
- Checks that the split page number is within the valid range of the PDF pages.

## How It Works

1. The script uses the `PyPDF2` library to read and manipulate PDF files.
2. The user provides:
   - The path to the input PDF file.
   - The directory to save the output files.
   - The page number where the PDF should be split.
3. The PDF is then divided into two parts:
   - **Part 1**: Pages from the start of the document up to (but not including) the split page.
   - **Part 2**: Pages from the split page to the end of the document.
4. The two parts are saved in the specified output directory as `part1.pdf` and `part2.pdf`.

## Requirements

- Python 3.x
- [PyPDF2](https://pypi.org/project/PyPDF2/) library

You can install `PyPDF2` using pip:
```bash
pip install PyPDF2
