# 🐔 End-to-End Chicken Disease Classification using Fecal Images

## 📌 Project Overview
This project aims to classify chicken diseases based on fecal images using deep learning techniques. By leveraging a Convolutional Neural Network (CNN), the model can detect and diagnose various poultry diseases, helping farmers take preventive measures in real time.

---

## 🚀 Features
- **Automated Disease Detection**: Identifies chicken diseases based on fecal images.
- **Deep Learning Model**: Uses CNN for accurate classification.
- **Logging & Monitoring**: Tracks model training and inference processes.
- **Preprocessing Pipeline**: Efficiently processes fecal images for improved predictions.
- **Scalable & Extensible**: Can be adapted for additional poultry diseases.

---

## 💂️ Workflows
1. Update `config.yaml`
2. Update `params.yaml`
3. Update the entity
4. Update the configuration manager in `src/config`
5. Update the components
6. Update the pipeline
7. Update `main.py`
8. Update `app.py`

---

## 💂️ Project Structure
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

---

## 🛠️ Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/Chicken-Disease-Classification-using-Fecal-Image.git
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

---

## 🏅 Training the Model
Run the following command to train the model:
```bash
python main.py
```

---

## 🔬 Testing the Model
Once the model is trained, you can test it on new fecal images using:
```bash
python predict.py --image_path sample.jpg
```

---

## 🛠️ Deployment: AWS CI/CD Pipeline with GitHub Actions

### 1️⃣ Login to AWS Console

### 2️⃣ Create IAM User with Specific Access
- **EC2 Access**: Virtual machine for hosting.
- **ECR**: Elastic Container Registry to store Docker images.

### 3️⃣ Build and Push Docker Image
1. Build Docker image of the source code.
2. Push Docker image to ECR.
3. Launch EC2 instance.
4. Pull the Docker image from ECR to EC2.
5. Run the Docker container on EC2.

### 4️⃣ AWS Policies Required
- `AmazonEC2ContainerRegistryFullAccess`
- `AmazonEC2FullAccess`

### 5️⃣ Create ECR Repository to Store Docker Image
- Save the URI: `566373416292.dkr.ecr.us-east-1.amazonaws.com/chicken`

### 6️⃣ Set Up EC2 Instance (Ubuntu) and Install Docker
```bash
sudo apt-get update -y
sudo apt-get upgrade -y
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
sudo usermod -aG docker ubuntu
newgrp docker
```

### 7️⃣ Configure EC2 as a Self-Hosted GitHub Runner
```
Settings > Actions > Runners > New self-hosted runner > Choose OS > Run the commands
```

### 8️⃣ Set Up GitHub Secrets for AWS Deployment
```plaintext
AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_REGION=us-east-1
AWS_ECR_LOGIN_URI=566373416292.dkr.ecr.ap-south-1.amazonaws.com
ECR_REPOSITORY_NAME=simple-app
```

---

## 📊 Logging & Monitoring
Logs will be stored in the `logs/` directory. To monitor logs in real-time:
```bash
tail -f logs/running_logs.log  # On macOS/Linux
type logs\running_logs.log  # On Windows
```

---

## 📚 Contributing
1. Fork the repository.
2. Create a new branch.
3. Make improvements.
4. Submit a pull request.

---

## 🐟 License
This project is licensed under the MIT License.

---

### 📩 Contact
For any inquiries, feel free to reach out via email or open an issue in the repository.

