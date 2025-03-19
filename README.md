# 🚀 Terraform AWS S3 Static Website Hosting

This project automates the setup of a **static website** hosted on **AWS S3** using Terraform.

## 📚 Features
- Creates an S3 bucket with public access.
- Uploads `index.html` and `error.html` with public-read ACL.
- Configures the bucket for static website hosting.
- Metadata added to prevent browser caching.

## 🛠️ Setup Instructions
1. **Clone the Repository:**
```bash
git clone <repo-url>
cd terraform-aws
```
2. **Initialize Terraform:**
```bash
terraform init
```
3. **Plan and Apply:**
```bash
terraform plan
terraform apply
```

## 📄 File Structure
- `main.tf` – Defines resources.
- `variables.tf` – Input variables.
- `outputs.tf` – Outputs bucket URL.

## 📄 Project Description
This project leverages Terraform to create an automated static website hosting solution using AWS S3. The HTML files (`index.html` and `error.html`) are uploaded to the bucket and public read access is granted using ACL. Bucket ownership and public access controls are properly configured. The website configuration points to the `index.html` as the default document and `error.html` for error handling.

## 🎯 Future Improvements
- Add CloudFront for content delivery.
- Integrate GitHub Actions for CI/CD.

