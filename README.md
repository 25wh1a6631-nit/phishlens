# 🛡️ PhishLens

A beginner-friendly web application that analyzes URLs for common phishing indicators and helps users identify potentially suspicious links.

## 🎯 Why PhishLens?

Phishing URLs can sometimes contain structural warning signs that aren't obvious at first glance.

PhishLens provides a simple way to inspect a URL and understand **why it may be suspicious** instead of only giving a final risk score.

## ✨ Features

- 🔍 URL validation
- 🛡️ Rule-based phishing detection
- 📊 Risk scoring
- 🟢 Low Risk / 🟡 Suspicious / 🔴 High Risk classification
- 🔬 Individual security-check breakdown
- ⚠️ Detection explanations
- 🛡️ Safety recommendations
- 🌐 Clean Streamlit web interface

## 🔎 What PhishLens Checks

PhishLens currently looks for:

- HTTPS usage
- Unusually long URLs
- IP addresses used instead of domain names
- Excessive subdomains
- Multiple hyphens in domains
- `@` symbols
- Excessive URL encoding
- Suspicious keywords such as `login`, `verify`, `account`, and `password`

Each detected indicator contributes to the overall risk score.

## 🧰 Tech Stack

- **Python**
- **Streamlit**
- **Regular Expressions**
- **Python URL Parsing**

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/phishlens.git
cd phishlens
```

### 2. Install dependencies

```bash
python -m pip install streamlit
```

### 3. Run the application

```bash
python -m streamlit run app.py
```

The application will open in your browser.

## 🧪 Example

Try analyzing:

```text
http://192.168.1.100/verify/account
```

PhishLens can identify multiple indicators, such as:

- No HTTPS
- IP address instead of a domain
- Suspicious keywords

The application then explains which checks were triggered.
## 📸 Preview

### URL Analysis
![PhishLens URL analysis](./phishlens-result.png)

### Detailed Security Checks
![PhishLens security check breakdown](./phishlens-details.png)

## ⚠️ Limitations

PhishLens is a **rule-based heuristic tool**.

A low-risk result does **not** guarantee that a website is safe, and a suspicious result does not necessarily prove that a website is malicious.

The project is intended for educational purposes and basic URL analysis.

## 🔮 Future Improvements

Potential future versions could include:

- More advanced URL analysis
- Domain reputation checks
- Threat-intelligence API integration
- Visualization of risk factors
- Improved scoring methodology
- Automated test cases
- Deployment as a public web application

## 👩‍💻 Project

Built as a beginner cybersecurity project to explore Python, web development, and defensive security concepts.
