<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Disease Detection and Diagnosis using Computer Vision</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      padding: 20px;
      max-width: 900px;
      margin: auto;
    }
    code {
      background-color: #f4f4f4;
      padding: 2px 4px;
      border-radius: 4px;
    }
    pre {
      background-color: #f4f4f4;
      padding: 10px;
      border-radius: 5px;
      overflow-x: auto;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-bottom: 1em;
    }
    table, th, td {
      border: 1px solid #ccc;
    }
    th, td {
      padding: 10px;
      text-align: left;
    }
    h1, h2, h3 {
      color: #2c3e50;
    }
    a {
      color: #3498db;
    }
  </style>
</head>
<body>

<h1>🩺 Disease Detection and Diagnosis using Computer Vision</h1>

<p>A deep learning-based healthcare application that leverages YOLO and Computer Vision techniques to detect and classify chest-related diseases (e.g., pneumonia, tuberculosis) from X-ray images. Built using Python, OpenCV, YOLOv5, and deployed via a Streamlit web app.</p>

<h2>📌 Project Overview</h2>
<ul>
  <li>✅ Detect chest anomalies using YOLOv5</li>
  <li>✅ Classify diseases with CNNs or pretrained models</li>
  <li>✅ Streamlit-based interactive web interface</li>
  <li>✅ Visualization with bounding boxes and confidence scores</li>
  <li>✅ Real-time predictions and batch processing support</li>
</ul>

<h2>🔍 Use Case</h2>
<p>Early detection of chest diseases such as:</p>
<ul>
  <li>Pneumonia</li>
  <li>Tuberculosis</li>
  <li>Cardiomegaly</li>
  <li>COVID-19 (optional)</li>
  <li>Normal (no abnormality)</li>
</ul>

<h2>📂 Project Structure</h2>
<pre>
disease-detection-cv/
├── data/
├── models/
├── notebooks/
├── src/
│   ├── detector.py
│   ├── classifier.py
│   ├── preprocessing.py
│   ├── utils.py
├── streamlit_app.py
├── requirements.txt
├── README.md
└── yolov5/
</pre>

<h2>⚙️ Features</h2>
<ul>
  <li>🔬 YOLOv5 Detection</li>
  <li>🧠 Classification</li>
  <li>🌐 Web App</li>
  <li>📊 Performance Metrics</li>
  <li>📸 Visualization</li>
</ul>

<h2>🛠️ Installation</h2>
<pre><code>git clone https://github.com/yourusername/disease-detection-cv.git
cd disease-detection-cv
pip install -r requirements.txt
</code></pre>

<p><strong>Download trained YOLOv5 weights</strong> and place them in the <code>models/</code> directory.</p>

<h2>🚀 Run the App</h2>
<pre><code>streamlit run streamlit_app.py</code></pre>

<p>Upload a chest X-ray image and get disease predictions with bounding boxes and confidence scores.</p>

<h2>📊 Model Training (Optional)</h2>
<ol>
  <li>Label dataset using Roboflow or LabelImg</li>
  <li>Convert to YOLO format</li>
  <li>Train YOLOv5:
<pre><code>python yolov5/train.py --img 640 --batch 16 --epochs 100 --data data.yaml --weights yolov5s.pt</code></pre>
  </li>
</ol>

<h2>🧪 Evaluation</h2>
<ul>
  <li>YOLOv5 Metrics: mAP@0.5, Precision, Recall</li>
  <li>Classification Metrics: Accuracy, ROC-AUC, Confusion Matrix</li>
  <li>Visual Results: Bounding boxes on test images</li>
</ul>

<h2>📈 Results</h2>
<table>
  <tr>
    <th>Disease</th>
    <th>Precision</th>
    <th>Recall</th>
    <th>F1 Score</th>
  </tr>
  <tr>
    <td>Pneumonia</td>
    <td>0.92</td>
    <td>0.89</td>
    <td>0.90</td>
  </tr>
  <tr>
    <td>Tuberculosis</td>
    <td>0.88</td>
    <td>0.87</td>
    <td>0.87</td>
  </tr>
  <tr>
    <td>Cardiomegaly</td>
    <td>0.90</td>
    <td>0.91</td>
    <td>0.90</td>
  </tr>
  <tr>
    <td>Normal</td>
    <td>0.95</td>
    <td>0.96</td>
    <td>0.95</td>
  </tr>
</table>

<h2>🧰 Tech Stack</h2>
<ul>
  <li>YOLOv5</li>
  <li>OpenCV</li>
  <li>PyTorch</li>
  <li>TensorFlow/Keras (optional)</li>
  <li>Streamlit</li>
  <li>Matplotlib, Seaborn</li>
  <li>Pandas, NumPy</li>
</ul>

<h2>📚 Dataset Sources</h2>
<ul>
  <li><a href="https://nihcc.app.box.com/v/ChestXray-NIHCC">ChestX-ray14 (NIH)</a></li>
  <li><a href="https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database">COVID-19 Radiography Dataset</a></li>
  <li><a href="https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia">Pneumonia Dataset</a></li>
</ul>

<h2>🙋‍♂️ Author</h2>
<p><strong>Saravanan</strong><br>
📧 <a href="mailto:saravananits4@gmail.com">saravananits4@gmail.com</a><br>
🌐 <a href="https://www.linkedin.com/in/itssaravanan" target="_blank">LinkedIn Profile</a></p>

<h2>📄 License</h2>
<p>This project is licensed under the MIT License - see the LICENSE file for details.</p>

</body>
</html>

