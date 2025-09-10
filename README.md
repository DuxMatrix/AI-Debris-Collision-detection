🛰️ AI Space Debris Collision Risk Detection
An Explainable AI (XAI) system that predicts and analyzes collision risks between space debris and satellites using machine learning and orbital data.

🌟 Features
Risk Classification: Predicts Low/Medium/High collision risk

Explainable AI: SHAP-based explanations for model decisions

Real Data Processing: Uses Celestrak satellite orbital data (TLE format)

Multiple ML Models: Compares Random Forest, XGBoost, LightGBM, CatBoost

Interactive Analysis: Query specific instances for detailed risk explanations

# Install dependencies
!pip install skyfield numpy pandas scikit-learn shap matplotlib scipy

# Run the complete analysis
from space_debris_ai import SpaceDebrisAnalyzer
analyzer = SpaceDebrisAnalyzer()
analyzer.run_full_analysis()

📊 Model Performance
Best Model: CatBoost Classifier (97.05% accuracy)

Precision: 96.8% (High Risk), 98.2% (Medium), 99.1% (Low)

Recall: 95.7% (High Risk), 97.5% (Medium), 99.3% (Low)

🔍 Example Output
🔍 Instance #45: HIGH RISK (96% confidence)
📋 Factors: 
   • Distance: 12.3km (increases risk by 0.82)
   • Relative Velocity: 14.5km/s (increases risk by 0.76)
   • Combined Size: 16.2m (increases risk by 0.68)
⚠️ Recommendation: Immediate evasive action recommended


🏗️ Architecture
Data Acquisition: Celestrak TLE data → Orbital parameters

Feature Engineering: Distance, velocity, size metrics

ML Training: Multiple classifier comparison

XAI Implementation: SHAP force plots and explanations

Interactive Interface: Instance-based query system

💡 Use Cases
Space traffic management and monitoring

Satellite collision avoidance systems

Space mission planning and risk assessment

Educational tool for orbital mechanics

🛠️ Requirements
Python 3.8+

skyfield, scikit-learn, shap, numpy, pandas, matplotlib

🤝 Contributing
Contributions welcome! Please feel free to submit a Pull Request.

