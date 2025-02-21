---
# **Automated Defect Recognition (ADR) System for Ordnance Factory**  

## **Project Overview**  
The **Automated Defect Recognition (ADR) System** is designed for the **Ordnance Factory Itarsi (OFI), Madhya Pradesh**,
to process and analyze **X-ray DICOM (.dcm) images** of ammunition components. This system **enhances defect detection** by
converting DICOM files into human-visible digital images through **high-pass filtering and Fourier transform techniques**.  

## **Technologies Used**  
- **Python** (NumPy, OpenCV, Pydicom, Skimage)  
- **Image Processing** (Fourier Transform, Gaussian High-Pass Filtering, Intensity Rescaling)  
- **DICOM File Handling** (Medical Imaging Standard)  

## **Key Features**  
✔ **DICOM Image Processing:** Converts X-ray DICOM files into **enhanced BMP images** for defect visualization.  
✔ **Gaussian High-Pass Filtering:** Removes low-frequency noise to **highlight fine defects** in ammunition components.  
✔ **Automated Metadata Extraction:** Saves **DICOM metadata** for reference and traceability.  
✔ **Fast & Scalable:** Optimized for quick processing of **high-resolution industrial X-ray images**.  

## **How It Works**  
1️⃣ **Load DICOM File:** The system reads the **X-ray scan** using Pydicom.  
2️⃣ **Apply Fourier Transform:** Converts the image into the frequency domain.  
3️⃣ **Apply Gaussian High-Pass Filter:** Enhances **edge details and defects**.  
4️⃣ **Inverse Transform & Rescaling:** Converts back to a human-readable **BMP image** with enhanced contrast.  
5️⃣ **Save Processed Image & Metadata:** The system **saves the filtered image** and extracts **DICOM metadata** into a text file.  

## **Installation & Usage**  
### **Installation**  
```bash
pip install numpy opencv-python pydicom scikit-image
```
### **Run the Script**  
```python
python process_dicom.py --file <input.dcm> --cutoff 80
```
- Replace `<input.dcm>` with your **DICOM file name**.  
- The **processed image** and **metadata file** will be saved automatically.  

## **Project Confidentiality**  
⚠️ **Note:** This project is developed for a **government defense facility** and follows strict security protocols. The code does not store or transmit data externally.  

## **License**  
🔒 **Private & Confidential - Restricted Usage**  

---
