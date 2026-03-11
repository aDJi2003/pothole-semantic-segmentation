# Pothole Semantic Segmentation

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Framework-PyTorch%20%7C%20HuggingFace-orange?style=for-the-badge&logo=pytorch)](https://huggingface.co/)

Repositori ini berisi implementasi solusi untuk kompetisi **Data Science ARA 7.0 (ITS)** oleh tim **Menang Kalah Tetap Nganggur**. Kami mengusulkan pendekatan *Ensemble* menggunakan dua arsitektur *State-of-the-Art* (SOTA), yaitu **SegFormer** dan **Mask2Former**, untuk mendeteksi lubang jalan pada kondisi citra yang bervariasi.

## Fitur Utama
- **Ensemble Modeling:** Sinergi antara **SegFormer** (efisiensi Transformer) dan **Mask2Former** (fleksibilitas Universal Architecture) untuk hasil segmentasi yang lebih presisi.
- **Adaptive Data Augmentation:** Penggunaan teknik augmentasi yang adaptif untuk menangani *heterogeneity* pada dataset (variasi cuaca, pencahayaan, dan sudut kamera).
- **Comprehensive EDA:** Analisis mendalam mengenai ketidakseimbangan kelas dan karakteristik visual jalanan.
- **Inference Optimization:** Strategi untuk menggabungkan *output* dari kedua model guna mendapatkan *mask* akhir yang optimal.

## Tech Stack
- **Deep Learning:** PyTorch, Hugging Face Transformers
- **Computer Vision:** Albumentations, OpenCV, Pillow
- **Data Analysis:** NumPy, Pandas, Matplotlib, Seaborn

## Struktur Notebook
Proyek ini disusun secara sistematis di dalam file `.ipynb`:
1. **Persiapan Lingkungan:** Setup library dan dependensi.
2. **Deskripsi Dataset:** Eksplorasi statistik dan visualisasi citra heterogen.
3. **Metodologi:**
    - Desain Arsitektur Model Ensemble.
    - Implementasi Augmentasi Data Ekstensif.
    - Konfigurasi Fungsi Kerugian (*Loss Function*).
4. **Evaluasi:** Komparasi kandidat model dan analisis hasil inferensi.
