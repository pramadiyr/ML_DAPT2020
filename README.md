# ML_DAPT2020: Intrusion Detection with AI

A comprehensive machine learning project demonstrating step-by-step how to build AI models for intrusion detection and APT (Advanced Persistent Threat) detection using the DAPT 2020 dataset.

## 🎯 Project Overview

This project showcases:
- **Data exploration and preprocessing** of network flow data
- **Binary classification** for intrusion detection (benign vs attack)
- **Feature engineering** and selection from CICFlowMeter features
- **Model evaluation** with multiple ML algorithms
- **Real-world cybersecurity applications**

## 📊 Results Achieved

- **🏆 97.6% Accuracy** with Random Forest classifier
- **📈 99.7% AUC-ROC** score (near-perfect discrimination)
- **🎯 95.1% Attack Detection Rate** (recall)
- **⚡ 1.5% False Positive Rate** (minimal false alarms)

## 📁 Project Structure

```
ML_DAPT2020/
├── data/csv/                    # DAPT 2020 dataset (10 CSV files)
├── notebooks/                  # Jupyter notebooks
│   └── 01_data_exploration.ipynb  # Main analysis notebook
├── scripts/                    # Python scripts (future)
├── results/                    # Model outputs and results
├── venv/                       # Virtual environment
├── requirements.txt            # Python dependencies
├── .gitignore                  # Git ignore rules
└── README.md                   # This file
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Git

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ML_DAPT2020.git
   cd ML_DAPT2020
   ```

2. **Set up virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Download DAPT 2020 dataset:**
   - Place the dataset CSV files in the `data/csv/` directory
   - The project expects 10 CSV files from the DAPT 2020 dataset

5. **Start exploring:**
   ```bash
   jupyter notebook notebooks/01_data_exploration.ipynb
   ```

## 📈 Key Features

### Data Processing
- ✅ Handles inconsistent CSV headers automatically
- ✅ Combines multiple dataset files seamlessly
- ✅ Comprehensive data quality assessment
- ✅ Advanced feature selection and correlation analysis

### Machine Learning
- 🤖 **Random Forest** and **Logistic Regression** models
- 🔍 **Feature importance analysis** for interpretability
- 📊 **ROC curve analysis** and performance metrics
- 🎯 **Binary classification** optimized for cybersecurity

### Visualizations
- 📈 Attack distribution across time and network segments
- 🔗 Feature correlation heatmaps
- 📊 Model performance comparisons
- 🎯 ROC curves for model evaluation

## 🛡️ Cybersecurity Applications

This project demonstrates practical applications for:
- **Network Security Monitoring** (SOC environments)
- **Automated Threat Detection** with low false positives
- **APT Early Warning Systems**
- **Network Traffic Analysis** for incident response

## 🔬 Technical Highlights

### Dataset Insights
- **86,691 network flows** from 5 days of traffic
- **13 different attack types** covering the APT kill chain
- **84 CICFlowMeter features** for comprehensive flow analysis
- **Multi-network coverage** (public, private, mixed segments)

### ML Pipeline
- **Feature Selection**: Reduced 79 features to 30 most informative
- **Class Balance**: 73.5% benign vs 26.5% attack traffic
- **Cross-validation**: Stratified splits maintaining class distribution
- **Scaling**: StandardScaler for optimal model performance

## 📚 Learning Path

1. **Data Exploration** → Understanding network flow patterns
2. **Preprocessing** → Feature engineering and selection
3. **Modeling** → Binary classification for intrusion detection
4. **Evaluation** → Performance metrics and visualization
5. **Next Steps** → Multi-class classification and APT staging

## 🤝 Contributing

Feel free to contribute by:
- Adding new ML models or techniques
- Implementing multi-class attack classification
- Creating deployment scripts for real-time detection
- Improving visualization and analysis

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- **DAPT 2020 Dataset** creators for providing comprehensive APT data
- **CICFlowMeter** for network flow feature extraction
- **Scikit-learn** community for excellent ML tools

## Steps
- Data exploration
- Preprocessing
- Simple binary classification (benign vs attack)

---


## 📥 Dataset Note

The DAPT 2020 dataset files are not included in this repository due to size constraints. To run the analysis:

1. Download the DAPT 2020 dataset from the official source
2. Place the CSV files in the `data/csv/` directory
3. The notebook will automatically detect and process all CSV files

Expected files:
- enp0s3-monday.pcap_Flow.csv
- enp0s3-monday-pvt.pcap_Flow.csv  
- enp0s3-tuesday.pcap_Flow.csv
- enp0s3-wednesday.pcap_Flow.csv
- enp0s3-thursday.pcap_Flow.csv
- enp0s3-friday.pcap_Flow.csv
- And additional network segment files

The project includes automatic header detection and correction for inconsistent CSV formats.
