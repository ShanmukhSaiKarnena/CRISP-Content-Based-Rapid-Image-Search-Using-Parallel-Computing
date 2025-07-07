# CRISP-Content-Based-Rapid-Image-Search-Using-Parallel-Computing
Implemented a Content-Based Image Retrieval (CBIR) system using feature extraction and Chi-Square distance. Compared sequential and multithreaded parallel processing (via ThreadPoolExecutor) to improve retrieval speed. Achieved significant speedup in image similarity search using Hu Moments and color histograms.


📌 Project Title:
CRISP – Content-Based Rapid Image Search Using Parallel Computing

🧠 Project Description:
CRISP is a Content-Based Image Retrieval (CBIR) system that enables searching for visually similar images by analyzing image content instead of relying on metadata or filenames. The system supports both sequential and parallel processing approaches and compares their efficiency in terms of processing speed and retrieval performance.

This project demonstrates how parallel computing can significantly improve the performance of large-scale image retrieval tasks using multithreading in Python.

🔍 Key Features:
🔹 Image Preprocessing:
Resizes images to 500×500 pixels

Converts images to grayscale

Applies Gaussian blur to reduce noise

Uses Laplacian sharpening to enhance edges

🔹 Feature Extraction:
Color Histogram (12×12×12 bins) to capture color distribution

Hu Moments to describe shape and geometric features

🔹 Similarity Comparison:
Uses Chi-Square Distance to measure similarity between the query image and dataset images

Lower distance = higher similarity


⚙️ Implementation Approaches:
1. Sequential Processing:
Reads each image one by one

Extracts features and computes similarity to query image

Sorts and displays top 5 most similar images

2. Parallel Processing:
Uses Python’s ThreadPoolExecutor for multithreading

Simultaneously processes multiple images to speed up retrieval

Achieves significant speedup over sequential version


⏱ Performance Evaluation:
Execution time is recorded for both methods

Speedup is calculated as:

ini
Copy
Edit
Speedup = Sequential Time / Parallel Time
Visualization includes:

Query image

Top 5 similar images with similarity scores (for both methods)

📈 Results & Conclusion:
Parallel processing reduced image retrieval time significantly

System scales well for large image datasets

Ideal for applications like image search engines, facial recognition, medical imaging, etc.

📁 Dataset Used:
INRIA Holidays Dataset – Kaggle

💻 Tools & Technologies:
Python

OpenCV

NumPy

Matplotlib

concurrent.futures (ThreadPoolExecutor)


🚀 How to Run:
bash
Copy
Edit
git clone https://github.com/your-username/CRISP--CBIR.git
cd CRISP--CBIR
pip install -r requirements.txt
python cbir_parallel.py   # or cbir_sequential.py


👨‍💻 Author:
Karnena Shanmukha Sai
B.Tech CSE, VIT Chennai
📧 karnena.shanmukha2022@vitstudent.ac.in
🔗 LinkedIn
