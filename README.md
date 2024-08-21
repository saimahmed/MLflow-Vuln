[Vuln replication-mlflow ver 2.1.1-prep by Saima.pdf](https://github.com/user-attachments/files/16695178/Vuln.replication-mlflow.ver.2.1.1-prep.by.Saima.pdf)
# MLflow-Vulnerability
MLflow LFI/RFI Vulnerability -CVE-2023-1177 - Reproduced
One of the most popular tools in a ML system is MLflow that is used for managing end-to-end machine learning lifecycle. I tested the security of MLflow and reproduced a combined Local File Inclusion/Remote File Inclusion vulnerability which can lead to a complete system or cloud provider takeover. MLflow versions before 2.2.1 are vulnerable to Local File Inclusion (LFI) due to insufficient sanitization of user input in the API for retrieving model versions and registered models. An adversary could exploit this to read arbitrary files on the server's filesystem.
# Impact:
1. Information disclosure of sensitive server files (e.g., configuration files, keys).
2. Potential system compromise if the attacker can gain unauthorized access to critical system files.
# Mitigation:
1. Upgrade to MLflow 2.2.1 or later (addresses the vulnerability).
2. Implement access control measures for your MLflow server.
