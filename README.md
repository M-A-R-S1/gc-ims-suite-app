# GC-IMS Suite Application

A comprehensive, standalone graphical user interface built in PySide6 and PyTorch for processing, visualizing, and analyzing Gas Chromatography-Ion Mobility Spectrometry (GC-IMS) data. 

This application allows users to easily manage GC-IMS projects, explore spectral peaks, build custom datasets, and train/utilize neural networks for classification tasks.

## FEATURES
* **Dataset Manager:** Create, open, and organize labels and assign GC-IMS spectra to these labels. 
* **Pre-Processing:** Preprocess GC-IMS spectra by cutting and applying noise reduction and smoothing filters.
* **Peak Explorer:** Automatic peak detection and interactive visualization of GC-IMS spectra and detected peaks.
* **Consensus Peaks:** Detect and manage consensus peaks across the project. 
* **Neural Network Integration:** Train and use a variational autoencoder (VAE) neural network for peak reconstruction.
* **Peak Classification:** Create a random-forest classifier and classify your GC-IMS spectra.
* **Open Source Project:** Modify and adjust the core application to your own needs.
* **Cross-Platform:** Runs on Windows, macOS, and Linux.

---

## GETTING STARTED (FOR DEVELOPPERS)

If you want to run the application from source or contribute to the code, follow these steps:

### 1. Clone the Repository
Open your terminal or command prompt and clone the project via Git:
```bash
git clone [https://github.com/M-A-R-S1/gc-ims-suite-app.git](https://github.com/M-A-R-S1/gc-ims-suite-app.git)
cd gc-ims-suite-app
```
<br>

### 2. Set up a Virtual Environment (Recommended)
It is highly recommended to use a virtual environment to manage dependencies:
```bash
python -m venv venv
```
<br>

### 3. Install Dependencies
Since this application uses PyTorch, please make sure that you have installed the CUDA Toolkit
(https://developer.nvidia.com/cuda-downloads).<br><br>
Install all required Python packages (PySide6, PyTorch, Pandas, etc.):
```bash
pip install -r requirements.txt
```

<br>

### 4. Run the App
Launch the application locally:
```bash
python app_launcher.py
```
<br>

### 5. Modify the app by your own liking
If you manage to get the application to work feel free to adjust the pyside6 application to your 
own needs.

---

## BUILDING A STANDALONE EXECUTABLE

You can freeze this Python application into a standalone executable that does not 
require Python to be installed on the host machine. You can use PyInstaller for this process.

### 1. Building process
Run the following command in the root directory of the project:
```bash
pip install pyinstaller
pyinstaller GC-IMS-Suite.spec
```

