# <img src="modlex_icon_64x64.png" alt="Icon" width="64"/> **MoDLEx: Modern Diffusion Length Extractor**

**MoDLEx** is a cross-platform graphical tool designed for researchers to analyze Electron Beam Induced Current (EBIC) data. It provides a workflow to extract the carrier diffusion length (L) from semiconductor materials using curve-fitting algorithms.

## **📺 Video Tutorial**

[Watch the Quick Start Guide on YouTube](https://www.google.com/search?q=YOUR_YOUTUBE_LINK_HERE)

## **✨ Key Features**
  
* **Dual-Image Analysis:** Load and compare EBIC and Secondary Electron (SE) images side-by-side to correlate electrical signals with topography.  
* **Real-Time Line Profiles:** Dynamic extraction of line profiles with adjustable averaging widths.  
* **Physics Modeling:** Support for power-law exponents (n=-0.5 or n=-1.5).  
* **Automated Fitting:** One-click fitting with user-defined constraints and guesses.  
* **Comprehensive Export:** Save high-resolution graphs, CSV raw data, or a full "Analysis Abstract" report in PNG or PDF format.

## **🚀 Installation**

MoDLEx is distributed as a standalone binary for easy use without needing a Python environment.

### **Download Software**

Go to the [Releases](https://github.com/ocakiroglu/modlex/releases) page to download the latest version for your OS:

* **Windows:** .exe  
* **macOS:** .dmg  
* **Linux:** .AppImage

### **Running from Source**

If you prefer to run the script directly:

1. Clone the repository:  
   git clone [https://github.com/ocakiroglu/MoDLEx.git](https://github.com/ocakiroglu/MoDLEx.git)

2. Install dependencies:  
   pip install PySide6 numpy pillow matplotlib scipy

3. Run the application:  
   python MoDLEx-v2\_1.py

## **🛠 Workflow**

1. **Load Images:** Import your EBIC and SE maps (TIFF, PNG, or JPG).  
2. **Setup View:** Adjust the Scan Line center and the Contact/Boundary edges using the interactive sliders.  
3. **Configure Fit:** Set your physical parameters (Long edge size, offsets, and power law exponent).  
4. **Perform Fit:** Click "PERFORM FIT" to visualize the results.  
5. **Export:** Export your findings as a standardized PDF abstract or CSV data.

## **🔬 Scientific Background**

MoDLEx fits your data to the fundamental EBIC decay model:

$I(x) = I_0 \cdot e^{-x/L} \cdot x^n + y_0$

where $L$ is the carrier diffusion length.


## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## 🙏 Acknowledgments

This code in GUI design stage was developed with coding assistance from **Google's Gemini**, **Github Copilot** and **Claude model via Perplexity**. 

