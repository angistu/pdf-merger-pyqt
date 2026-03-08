# PDF Merger Desktop App

A simple desktop application for merging multiple PDF files into a single document.
This tool is built using **Python** and **PyQt5** and provides an intuitive graphical interface for organizing and previewing PDF files before merging them.

The application is designed to make merging PDF files easier without requiring command-line tools.

---

# Features

* Merge multiple PDF files into a single document
* Drag-and-drop file ordering
* Remove files from the merge list
* Preview PDF pages before merging
* Custom output filename
* Select custom output folder
* Progress indicator during merge process
* Restart / reset session quickly

---

# Requirements

The application requires:

* Python **3.9 or newer**
* PyQt5
* PyMuPDF (fitz)
* PyPDF2
* qdarktheme (optional, for UI theme)

---

# Installation

### 1. Clone the repository

```
git clone git@github.com:angistu/pdf-merger-pyqt.git
cd pdf-merger-app
```

### 2. Create a virtual environment (recommended)

Windows:

```
python -m env venv
env\Scripts\activate
```

Linux / macOS:

```
python3 -m env venv
source env/bin/activate
```

### 3. Install dependencies

```
pip install -r requirements.txt
```

If you do not have `requirements.txt`, install manually:

```
pip install PyQt5 PyMuPDF PyPDF2
```

---

# Running the Application

Run the application using:

```
python src/pdf_merger.py
```

The GUI window will open and you can start merging PDF files.

---

# How to Use

### 1. Add PDF Files

Click **"Pilih File PDF"** to select one or multiple PDF files from your computer.

You can add files multiple times if needed.

---

### 2. Arrange File Order

Drag the files inside the list to change the merge order.

The final PDF will follow this order.

---

### 3. Remove Files

Double-click a file in the list to remove it from the merge queue.

---

### 4. Choose Output Folder

Click **"Pilih"** next to *Lokasi Penyimpanan* and select the folder where the merged PDF will be saved.

---

### 5. Set Output File Name

Enter the name of the output PDF in the **Nama File** field.

Example:

```
merged_document
```

The program will generate:

```
merged_document.pdf
```

---

### 6. Merge the PDFs

Click **"Gabungkan"**.

The application will:

1. Combine all selected PDF files
2. Save the merged document to the selected folder
3. Display a completion message when finished

---

### 7. Restart / Reset

Click **"Restart"** to clear all loaded files and start a new merge session.

---

# Project Structure

Example project structure:

```
pdf-merger-app
│
├── src
│   └── pdf_merger.py
│
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

---

# Libraries Used

* **PyQt5** — Graphical User Interface
* **PyMuPDF (fitz)** — Rendering PDF pages for preview
* **PyPDF2** — Merging PDF files

---

# Future Improvements

Possible improvements for future versions:

* Drag & drop files directly from file explorer
* Show only first-page preview for faster performance
* Real-time merge progress indicator
* Export application as a standalone executable
* Support for splitting PDF files

---

# License

This project is licensed under the **MIT License**.

You are free to use, modify, and distribute this software.

---

# Author

Developed by Angistu Palamarta
