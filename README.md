## CloudWatch Sentinel

CloudWatch Sentinel is an anomaly detection system designed to identify malicious activities in AWS CloudWatch logs using the Isolation Forest algorithm. 

The project uses a dataset of 5,000 samples with 5,035 features. The data is split into a training set of 4,000 samples (2,048 normal and 1,952 malicious) and a test set of 1,000 samples (512 normal and 488 malicious).

The baseline Isolation Forest model achieved **62% accuracy**, with a precision of **58%** and recall of **92%** for normal events, but only **31% recall** for malicious anomalies. After hyperparameter tuning, the model's accuracy dropped to **51%**, maintaining perfect recall for normal events but failing to detect anomalies effectively.

Severity scoring is applied to flag detected anomalies by tier — critical, high, medium, and low — based on their anomaly scores, allowing prioritization of incident response.

This project showcases practical skills in:
- Data preprocessing and feature encoding for high-dimensional datasets.
- Implementing and tuning Isolation Forest for anomaly detection.
- Evaluation using confusion matrices, classification reports, and F1-scores.
- Severity tiering for actionable alerting.
- Preparing machine learning models for deployment on AWS Lambda for real-time monitoring.

The quantifiable results provide insights into the challenges of anomaly detection in cybersecurity datasets and demonstrate steps towards improving detection performance.

