# ☁️ AWS Cloud Incident Response | Cloud Security Investigation

## 📌 Project Overview

This project demonstrates a simulated AWS cloud security incident investigation in an AWS sandbox environment.

The project focuses on identifying suspicious IAM activities, investigating potential privilege escalation, analyzing S3 data access, and detecting attempts to disable or delete CloudTrail logging.

The investigation uses AWS IAM, AWS CloudTrail, Amazon CloudWatch Logs Insights, and Amazon S3.

The main objective is to reconstruct the incident timeline, identify security weaknesses, assess potential impact, and recommend remediation measures.

---

## 🎯 Project Objectives

- Investigate suspicious IAM user creation and permission changes.
- Identify potential privilege escalation through administrative permissions.
- Analyze IAM and S3 reconnaissance activities.
- Investigate suspicious access to sensitive test data in S3.
- Detect attempts to disable or delete CloudTrail logging.
- Reconstruct the incident timeline using cloud audit logs.
- Identify Indicators of Compromise (IOCs).
- Recommend incident containment and security improvements.

---

## 🛠️ Technologies & Tools Used

| Technology | Purpose |
|---|---|
| AWS IAM | Identity and access management investigation |
| AWS CloudTrail | Cloud activity logging and event analysis |
| Amazon CloudWatch Logs Insights | Log searching and investigation |
| Amazon S3 | Storage and test data investigation |
| AWS Management Console | Cloud environment configuration |
| AWS Athena | Cloud log analysis, where applicable |

---

## 🏗️ Project Architecture

```text
             AWS SANDBOX ENVIRONMENT
                       |
        +--------------+--------------+
        |              |              |
       IAM             S3          CloudTrail
        |              |              |
  User Creation    Test Data      Activity Logs
  Permissions      Log Storage         |
        |              |              |
        +--------------+--------------+
                       |
                 CloudWatch
                Logs Insights
                       |
             Incident Investigation
                       |
        +--------------+--------------+
        |              |              |
    Timeline       IOC Analysis    Impact
    Analysis                       Assessment
                       |
              Remediation Plan
                       |
              Security Hardening
```
