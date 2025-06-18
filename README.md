# 🌐 Static Website on AWS S3

## 📌 Overview
This project demonstrates how to host a static website using **Amazon S3**. The website is publicly accessible, and can optionally be linked to a custom domain using **Route 53** and **CloudFront** for CDN.

---

## 🛠️ Tools Used
- AWS S3 (Simple Storage Service)
- IAM (Permissions)
- Route 53 (Optional for domain)
- CloudFront (Optional for CDN)

---

## 🚀 Steps to Deploy

### 1. Create S3 Bucket
- Name must be globally unique (e.g., `my-static-web-demo`)
- Uncheck "Block All Public Access"
- Enable **Static Website Hosting**

### 2. Upload Files
- Upload `index.html` and any other assets
- Set correct MIME types (HTML, CSS, JS)

### 3. Apply Bucket Policy
Apply `s3_bucket_policy.json` in the Permissions tab to allow public access.

### 4. Test the Site
- Visit the **Bucket Static Website Endpoint** URL
- It should show your HTML content

---

## 🌐 Optional: Custom Domain Setup
If you have a domain:
- Use **Route 53** to create a hosted zone
- Point to your S3 endpoint using an alias record
- Optionally add **CloudFront** for HTTPS and faster delivery

---

## 🧠 Learnings
- Hosting static sites on AWS without a server
- Managing public access and bucket policies
- Optional integration with DNS and CDN

---

## 📸 Screenshot
![Website Screenshot](link-to-your-screenshot.png)

---

## 📎 Resources
- [AWS S3 Static Website Hosting Guide](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html)
