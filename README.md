# Chicken Disease Classification using Fecal Image

<<<<<<< HEAD
This project aims to classify chicken diseases using fecal images with the help of machine learning techniques.

## Workflows

1.Update config.yaml
2.Update params.yaml
3.Update the entity
4.Update the configuration manager in src config
5.Update the components
6.Update the pipeline
7.Update the main.py
8.Update the app.py

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model](#model)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Early detection of diseases in chickens is crucial for maintaining healthy poultry. This project leverages image processing and machine learning to classify diseases based on fecal images.

## Dataset
The dataset consists of fecal images collected from various sources. Each image is labeled with the corresponding disease.

## Installation
To get started, clone the repository and install the required dependencies:
```bash
git clone https://github.com/yourusername/Chicken-Disease-Classification-using-Fecal-Image.git
cd Chicken-Disease-Classification-using-Fecal-Image
pip install -r requirements.txt
```

## Usage
To train the model, run:
```bash
python train.py
```
To evaluate the model, run:
```bash
python evaluate.py
```
# AWS-CICD-Deployment-with-Github-Actions
## 1. Login to AWS console.
## 2. Create IAM user for deployment

#with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


#Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

#Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess

## 3. Create ECR repo to store/save docker image

Save the URI: 566373416292.dkr.ecr.us-east-1.amazonaws.com/chicken

# 4. Create EC2 machine (Ubuntu)
# 5. Open EC2 and Install docker in EC2 Machine:

#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

# 6. Configure EC2 as self-hosted runner:
setting>actions>runner>new self hosted runner> choose os> then run command one by one


## Model
The model is built using convolutional neural networks (CNNs) to extract features from the images and classify them into different disease categories.

## Results
The model achieves an accuracy of X% on the test dataset. Detailed results and analysis can be found in the `results` directory.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
=======
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


>>>>>>> 052e2b1c63426853c89a61c7d041e7d065d2f90f
