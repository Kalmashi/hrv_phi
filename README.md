# Golden Ratio in Heart Rate Data 

A Python-based analysis of heart rate variability (HRV) data from the PhysioNet **Meditation Data Set**.  
This notebook processes files, extracts heart rate data, and performs spectral analysis using Welch’s method. The notebook provides plots 
of heart rate time series, heart rate spectra and peaks. The code computes ratios using the highest peaks, and exports this data via csv for later 
comparison and analysis.  

The notebook shows that data for the subjects in the 2 meditating groups have HR spectra with top peaks in the golden ratio.
This is evident for individuals in these groups both before and during meditation. There are zero or few subjects 
in the remaining control groups that show this phenomenon. This is interesting because it demonstrates that the golden ratio 
is not just in nature's forms and man-made architecture. The golden ratio is in sound and other signal data. The golden ratio is 
in pairs of plasma waves from the Sun, both frequency and amplitude [doppler data] and in the tone of some people's voices. 


---

## 📀 Data Source

The dataset is from:

> Peng, C.-K., Mietus, J. E., Liu, Y., Khalsa, G., Douglas, P. S., Benson, H., & Goldberger, A. L. (1999).  
> *Exaggerated heart rate oscillations during two meditation techniques.*  
> **American Journal of Cardiology, 83(5): 877–878.**  
> Available via [PhysioNet](https://physionet.org/content/meditation/1.0.0/)

---

## 🏃🏻‍♂️‍ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Kalmashi/HR.git
   cd HR
2. Install dependencies
   pip install -r requirements.txt
3. Launch Jupyter Notebook
4. Open and run the notebook cells in order to reproduce the analysis 

---

## 🔮 Methods
The workflow includes:
- Downloading files from PhysioNet (if not already cached locally)
- Extracting heart rate data from &lt;code&gt; blocks
- Computing RR intervals
- Interpolating unevenly spaced heartbeats using cubic interpolation
- Computing the power spectral density (PSD) using Welch’s method
- Identifying spectral peaks and calculating ratios

---

## ✏️ Citation
If you use this dataset or analysis, please cite:

>Peng, C.-K., Mietus, J. E., Liu, Y., Khalsa, G., Douglas, P. S., Benson, H., & Goldberger, A. L. (1999).
>Exaggerated heart rate oscillations during two meditation techniques.
>Am J Cardiol, 83(5): 877–878.
>DOI: 10.1016/S0002-9149(98)01000-0

---

## 🧷 Dependencies
Main Python packages used:
- numpy
- pandas
- matplotlib
- scipy
- requests
- re

To install all dependencies:
pip install -r requirements.txt
  
---

## 😎 Author
Developed by Denisa Borges
📧 Contact: denisa.borges@gmail.com
GitHub: https://github.com/Kalmashi

---

## 🏁 License
This project is open-sourced under MIT License.

