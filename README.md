🚀 LSTM-Based Placement Prediction Model






📌 Overview

This project uses a Long Short-Term Memory (LSTM) neural network to predict placement outcomes for students based on historical trends, academic performance, and skills. The model provides placement probabilities, expected salary brackets, and skill recommendations.

🎯 Features

✅ Automated Dataset Loading from Google Drive 📂✅ LSTM Deep Learning Model for sequential data processing 🤖✅ Handles Large Datasets Efficiently 📊✅ Dropout & Batch Normalization for stability ⚖️✅ GPU-Accelerated Training in Google Colab ⚡✅ Performance Visualizations for accuracy, loss, and predictions 📉

📂 Dataset Requirements

The dataset should be in CSV format and contain the following:

Features: cgpa, iq, internship_experience, technical_skills, etc.

Target Variable: placement (1 = Placed, 0 = Not Placed)

🛠 Installation & Setup

1️⃣ Run on Google Colab

Upload placement-dataset.csv to Google Drive

Open Google Colab and enable GPU acceleration:Runtime → Change runtime type → Select GPU

Copy and run the following script:

# Mount Google Drive
from google.colab import drive
drive.mount('/content/drive')

# Install required dependencies
!pip install tensorflow numpy pandas seaborn matplotlib scikit-learn

2️⃣ Clone the Repository (Local Usage)

git clone https://github.com/your-username/lstm-placement-prediction.git
cd lstm-placement-prediction
pip install -r requirements.txt

🚀 Model Training & Prediction

Run the LSTM model training script:

python train.py  # (if running locally)

📊 Visualizations

The model generates the following plots:

Training & Validation Loss

Training & Validation Accuracy

Prediction Probability Distribution

📌 Sample Output

🔹 Test Accuracy: 91.5%
🔹 Sample Predictions:
CGPA: 8.5, IQ: 120, Actual: 1, Predicted: 1 (Probability: 0.89)
CGPA: 7.2, IQ: 110, Actual: 0, Predicted: 0 (Probability: 0.34)

🏆 Contributing

Feel free to contribute! Fork the repo and submit a Pull Request.

📜 License

This project is licensed under the MIT License.

