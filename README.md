# phishing-website-detection

This project analyzes a dataset containing information about URLs and uses machine learning algorithms to classify whether a URL is potentially malicious or not.

## Dataset

The dataset contains the following columns:

- `protocol`: The protocol used for the URL (e.g., http, https).
- `domain_name`: The domain name of the URL.
- `address`: The address portion of the URL.
- `long_url`: Boolean indicating if the URL is long.
- `having_@_symbol`: Boolean indicating if the URL contains the "@" symbol.
- `redirection_//_symbol`: Boolean indicating if the URL contains the "//" symbol.
- `prefix_suffix_separation`: Boolean indicating if the URL contains prefix and suffix separation.
- `sub_domains`: The number of subdomains in the URL.
- `having_ip_address`: Boolean indicating if the URL contains an IP address.
- `shortening_service`: Boolean indicating if the URL is shortened.
- `https_token`: Boolean indicating if the URL contains an HTTPS token.
- `abnormal_url`: Boolean indicating if the URL is abnormal.
- `web_traffic`: The amount of web traffic associated with the URL.
- `domain_registration_length`: The length of domain registration.
- `age_of_domain`: The age of the domain.
- `dns_record`: Boolean indicating if the URL has a DNS record.
- `statistical_report`: Binary label indicating if the URL is potentially malicious (1) or not (0).

## Data Preprocessing

- The dataset is loaded using pandas.
- Columns related to the URL structure are selected for analysis.
- The dataset is split into training and testing sets.

## Machine Learning Models

### Random Forest Classifier

- A Random Forest Classifier is trained on the training data.
- Predictions are made on the testing data.
- Accuracy and confusion matrix are computed for evaluation.

### Support Vector Machine (SVM)

- A Support Vector Machine (LinearSVC) classifier is trained on the training data.
- Predictions are made on the testing data.
- Accuracy and confusion matrix are computed for evaluation.

## Results

- The Random Forest Classifier achieved an accuracy of [accuracy_rf]%.
- The Support Vector Machine achieved an accuracy of [accuracy_svm]%.
- A comparison bar chart is plotted to visualize the performance of the two models.

## Dependencies

- Python 3.x
- pandas
- scikit-learn
- seaborn
- matplotlib

## Usage

1. Ensure all dependencies are installed.
2. Download the dataset and update the file path in the script.
3. Run the Python script to perform data analysis and model training.
4. View the results and evaluation metrics.
