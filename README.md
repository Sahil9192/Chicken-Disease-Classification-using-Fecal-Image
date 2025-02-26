# Chicken Disease Classification using Fecal Image

## 📌 Project Overview
This project aims to classify chicken diseases based on fecal images using deep learning techniques. By leveraging a Convolutional Neural Network (CNN), the model can detect and diagnose various poultry diseases, helping farmers take preventive measures in real time.

## 🚀 Features
- **Automated Disease Detection**: Identifies chicken diseases based on fecal images.
- **Deep Learning Model**: Uses CNN for accurate classification.
- **Logging & Monitoring**: Tracks model training and inference processes.
- **Preprocessing Pipeline**: Efficiently processes fecal images for improved predictions.
- **Scalable & Extensible**: Can be adapted for additional poultry diseases.

## 📂 Project Structure
```
Chicken-Disease-Classification-using-Fecal-Image/
│-- src/
│   ├── cnnClassifier/
│   │   ├── components/
│   │   ├── config/
│   │   ├── constants/
│   │   ├── entity/
│   │   ├── pipeline/
│   │   ├── utils/
│   │   ├── __init__.py
│   ├── main.py
│-- logs/
│-- artifacts/
│-- config/
│-- notebooks/
│-- venv/
│-- README.md
│-- requirements.txt
```

## 🛠️ Installation
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Sahil9192/Chicken-Disease-Classification-using-Fecal-Image.git
cd Chicken-Disease-Classification
```

### 2️⃣ Create a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate  # On Windows
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

## 🏋️ Training the Model
Run the following command to train the model:
```bash
python main.py
```

## 📊 Logging
Logs will be stored in the `logs/` directory. To monitor logs in real time:
```bash
tail -f logs/running_logs.log  # On macOS/Linux
type logs\running_logs.log  # On Windows
```

## 🔬 Testing the Model
Once the model is trained, you can test it on new fecal images using:
```bash
python predict.py --image_path sample.jpg
```

## 📖 Contributing
1. Fork the repository.
2. Create a new branch.
3. Make improvements.
4. Submit a pull request.

## 📜 License
This project is licensed under the MIT License.

---

### 📩 Contact
For any inquiries, feel free to reach out via email or open an issue in the repository.


