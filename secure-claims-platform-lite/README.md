# Secure Claims Platform Lite (SCPL)

SCPL is a **serverless, event-driven insurance claims processing system** designed to simulate a production-ready AWS environment for secure, scalable, and auditable claim handling.  
This project mirrors my cloud engineering skill set while remaining small enough to run in a personal AWS account.

---

## **📌 Use Case**
Insurance companies need a **fast, secure, and auditable** way to validate, store, and process claims. SCPL ingests claims via API, validates them through Lambda, stores them in DynamoDB, and securely backs up raw data in S3 (with KMS encryption). Metrics and dashboards provide operational visibility.

---

## **🛠 AWS Services Used**
- **API Gateway** – HTTP API entrypoint
- **EventBridge** – Event routing between API and Lambda
- **Lambda** – Claim validation and secure data processing
- **DynamoDB** – Claims metadata store
- **S3 + KMS** – Secure raw data archive
- **CloudWatch** – Logs, metrics, and dashboard
- **IAM** – Role-based and tag-based access control

---

## **🚦 Project Roadmap**
### **Week 0 – Setup**
- [x] Create repo, folder structure, and initial README
- [x] Define use case and AWS services
- [x] Prepare documentation structure

### **Week 1 – Core Pipeline**
- [ ] DynamoDB table (dev env)
- [ ] Lambda claim validation function
- [ ] EventBridge rule and bus
- [ ] API Gateway integration
- [ ] End-to-end test + screenshots

### **Week 2 – Security & Observability**
- [ ] KMS encryption for S3 backups
- [ ] CloudWatch custom metrics
- [ ] Dashboard creation
- [ ] IAM ABAC & SCP samples

---

## **📂 Folder Guide**
- `envs/dev` → Terraform configs for dev environment
- `lambda` → Lambda function source code
- `modules` → (optional) reusable Terraform modules
- `policies` → Custom IAM policy JSONs
- `cloudwatch` → Dashboards & alarms
- `docs/screenshots` → Deployment & test evidence
- `docs/PROJECT_STORY.md` → Full project narrative
- `docs/ARCHITECTURE_NOTES.md` → Design decisions

---

## **📸 Screenshots**
*(To be added in Week 1 & 2)*

---

## **⚖ License**
MIT License – free to use, modify, and share.
