# Predicting Eligibility for NSAP Schemes Using Machine Learning

This project aims to streamline the assignment of NSAP (National Social Assistance Programme) benefits to eligible citizens using machine learning techniques. It uses demographic and socio-economic data to predict which scheme a person qualifies for, enabling faster and more accurate assistance delivery.

## 👨‍💻 Developed By
**Bhanu Sharma**  
B.Tech CSE, Medi-Caps University

---

## 📌 Problem Statement

Manual verification of applications for NSAP schemes is time-consuming, error-prone, and delays support to beneficiaries such as the elderly, widows, and persons with disabilities. The goal is to automate this process using machine learning to predict the correct scheme for each applicant.

---

## ✅ Proposed Solution

### 🔹 Dataset
- **Source:** [AI Kosh](https://aikosh.indiaai.gov.in/web/datasets/details/district_wise_pension_data_under_the_national_social_assistance_programme_nsap_1.html)
- **Time Period:** 2025–2026
- **Target Variable:** `schemecode`
- **Features:**  
  `finyear`, `lgdstatecode`, `statename`, `lgddistrictcode`, `districtname`, `totalbeneficiaries`, `totalmale`, `totalfemale`, `totaltransgender`, `totalsc`, `totalst`, `totalgen`, `totalobc`, `totalaadhaar`, `totalmpbilenumber`

### 🔹 Data Preprocessing (via IBM AutoAI)
- Automatic missing value handling and outlier treatment
- Feature selection and scaling
- Categorical encoding (e.g., for state, gender)
- Low-impact features were dropped automatically

### 🔹 Model Development
- **Best Model:** Random Forest Classifier
- **Accuracy Achieved:** 98.4%
- Other models evaluated: Logistic Regression, Decision Trees, XGBoost
- Multi-class classification for scheme prediction

---

## 🚀 Deployment

- **Platform:** IBM Watson Studio (IBM Cloud Lite)
- **Tool Used:** IBM AutoAI
- **Deployment Type:** REST API (generated via Deployment Space)
- **Interface:** No-code, user-friendly deployment

---

## ⚙️ System Requirements

- IBM Cloud Lite Account
- IBM Watson Studio with AutoAI enabled
- NSAP dataset (.csv)
- (Optional) Python with `pandas`, `scikit-learn` for local testing

---

## 📈 Results

- **Accuracy:** 98.4%
- Evaluation through ROC curve, Precision vs Recall curve
- AutoAI leaderboard used for model selection

---

## 🔍 Conclusion

- The model demonstrates high reliability for real-world applications
- Enables faster scheme assignments with minimal manual intervention
- Scalable, adaptable, and cost-effective
- Developed using a no-code approach with IBM AutoAI

---

## 🌐 Future Scope

- Integrate Aadhaar and ration card verification APIs
- Add explainability layer (e.g., SHAP) to justify predictions
- Build a chatbot using Watson Assistant for user support

---

## 📚 References

- [AI Kosh – NSAP Dataset](https://aikosh.indiaai.gov.in)
- [IBM Cloud Documentation](https://cloud.ibm.com/docs)
- [IBM AutoAI Documentation](https://cloud.ibm.com/docs/watsonx?topic=watsonx-autoai-overview)
- [Scikit-learn – RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
- [NSAP Official Website](https://nsap.nic.in)

---

## 📎 GitHub Repository

🔗 [Click here to view the repository](https://github.com/BHANUSHARMA8319/Edunet_Skillbuild_IBM)

---

## 🏷️ License

This project is open-source under the [MIT License](LICENSE).

