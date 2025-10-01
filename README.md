# Real-Time Facial Expression and Age/Gender Analyzer

Welcome to the **Real-Time Facial Analyzer**! This is a single-page web application built with **HTML, JavaScript, and Tailwind CSS** that uses advanced AI models (`face-api.js` / TensorFlow.js) to perform real-time analysis of a face via a webcam or uploaded image.

## ✨ Key Features

| Feature | Description | 
 | ----- | ----- | 
| **Live Analysis** | Real-time detection of expressions, age, and gender. | 
| **Visual Overlay** | Draws a **bounding box** and labels (with emojis) directly onto the face. | 
| **Detailed Metrics** | Displays the probability of all 7 emotions using **attractive progress bars**. | 
| **Landmark Tracking** | Toggle to view the 68 key points the AI uses to track facial features. | 
| **Mobile-Ready** | Fully responsive layout that adjusts for phone screens. | 

---

## 🛠️ Setup and Installation (Required)

Because this app accesses your webcam and loads local AI models, it **must** be run from a local web server for security reasons.

1.  **Download Files:** Place your `index.html`, `README.md`, and `LICENSE` into your main project folder (e.g., `FacialDetector`).

2.  **Model Files:** Create a subfolder named **`models`** inside your project folder. This is the most crucial step—all 8 model files must be in this folder and named **EXACTLY** as shown below:

| Model Name (Manifest) | Model Data Shard | 
 | ----- | ----- | 
| `age_gender_model-weights_manifest.json` | **`age_gender_model-shard1`** | 
| `face_expression_model-weights_manifest.json` | **`face_expression_model-shard1`** | 
| `face_landmark_68_model-weights_manifest.json` | **`face_landmark_68_model-shard1`** | 
| `tiny_face_detector_model-weights_manifest.json` | **`tiny_face_detector_model-shard1`** | 

***Note: The `*-shard1` files MUST have no file extension (no `.json`).***

3.  **Start Local Server (Python 3):**
    * Open your terminal/command prompt and navigate to the `FacialDetector` directory.
    * Run the command: `python -m http.server 8000`

4.  **Launch:** Open your web browser and navigate to: `http://localhost:8000/index.html`

---

## 👤 Contact Information

| Detail | Value | 
 | ----- | ----- | 
| **Name** | K. Sudarsan | 
| **Phone** | 7730829186 | 