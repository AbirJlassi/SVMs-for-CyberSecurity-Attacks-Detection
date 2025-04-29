# IoT Attack Detection using SVM and the TON_IoT Dataset

This project applies **Support Vector Machines (SVM)** to detect malicious activities in IoT environments using the **TON_IoT dataset**. It addresses binary and multi-class classification problems, incorporates class imbalance handling techniques (e.g., SMOTE).

---

## 📌 Objective

To build and evaluate SVM model capable of:
- Distinguishing between normal and malicious IoT behavior (binary classification)
- Identifying specific **types of attacks** (multi-class classification)
- Reducing **false positives** to minimize unnecessary alerts

---

## 🧠 Dataset: TON_IoT

- **Name**: Telecommunications and Operational Network dataset for Internet of Things (TON_IoT)
- **Source**: [UNSW Canberra Cyber](https://research.unsw.edu.au/projects/toniot-datasets)
- **Types of Data**:
  - Telemetry from IoT devices
  - Operating system logs (Windows, Linux)
  - Network traffic features
- **Labels**: Includes binary labels (normal vs attack) and multiple attack categories (Backdoor, DDoS, Injection, Ransomware, etc.)

---

## Techniques Used

### Support Vector Machines (SVM)
- Linear and RBF kernels
- Binary and multi-class configurations
- Hyperparameter tuning with GridSearchCV

### Feature Selection
- **Mutual Information**: For detecting linear and non-linear relevance with the target

### Class Imbalance Handling
- Used **SMOTE (Synthetic Minority Oversampling Technique)** to generate synthetic examples of underrepresented attack classes
- Improved recall and reduced model bias

### ⚔️ Multi-Class Classification
- Applied SVM with **One-vs-One** strategy
- Goal: Classify the exact type of attack (e.g., ransomware vs DDoS)

---


