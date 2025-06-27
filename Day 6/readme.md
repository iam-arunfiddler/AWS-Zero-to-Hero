# 📦 Day 6 - Master AWS S3 | AWS Zero to Hero - Tamil

Welcome to **Day 6** of the **AWS Zero to Hero - Tamil** series by **Arun Fiddler**!  
In this session, we explored **Amazon S3 (Simple Storage Service)** — a foundational AWS service used for object storage — and discussed everything you need to know to get hands-on and production-ready with S3.
---
🎥 Complete Playlist on Youtube : https://www.youtube.com/watch?v=prkYvd94EGM&list=PLpGbJOX1pnPzEK8BsXoLdgSdk0qEq9D-x


## 🎯 What You Will Learn

In this session, we covered:

- ✅ What is Amazon S3?
- ✅ How S3 achieves massive scalability, durability, and high availability
- ✅ Creating and configuring S3 buckets step-by-step
- ✅ S3 object fundamentals — uploading, organizing, and accessing files
- ✅ Understanding and fixing common errors like **403 Access Denied**
- ✅ Bucket policies and public access configuration
- ✅ Hosted and accessed a **3-tier architecture image** publicly from S3
- ✅ Pulled a working public bucket policy from GitHub to debug access issues
- ✅ S3 security layers — IAM, bucket policies, and block public access
- ✅ Real-world best practices

---

## 🧠 What is Amazon S3?

Amazon S3 is an **object storage service** that allows you to store and retrieve any amount of data from anywhere on the web. It is designed for:

- 🧠 **99.999999999% durability** (11 9’s)
- 🌍 **Scalability without limits**
- 🔐 **Granular security control**
- ⚡ **High availability and performance**

Use cases include:
- Backups & Archives
- Big data analytics
- Application data storage
- File distribution (images, PDFs, media, etc.)

---

## 🏗️ Core Concepts Covered

| Concept | Explanation |
|--------|-------------|
| **Buckets** | Top-level storage containers; each must have a unique name globally |
| **Objects** | Files stored in buckets (e.g., images, documents, backups) |
| **Regions** | Choose where your data is stored geographically for latency and compliance |
| **Storage Classes** | Decide cost/performance trade-offs: Standard, Intelligent-Tiering, Glacier, etc. |
| **Access Permissions** | Manage using IAM, bucket policies, and ACLs (not recommended) |
| **Public Access Settings** | Explained how "Block Public Access" affects accessibility |
| **URLs** | Object URLs follow the format: `https://bucket-name.s3.amazonaws.com/object-key` |

---

## 🛠️ Demo: Hosting a 3-Tier Architecture Image on S3

To demonstrate public access and permissions, we uploaded a **3-tier architecture diagram** and accessed it publicly using its **S3 object URL**.

Steps:

1. Created a new S3 bucket
2. Uploaded the image (e.g., `3-tier-arch.png`)
3. Attempted to access the image URL and encountered: ❌ **403 Access Denied**
4. Diagnosed the issue: bucket was private by default and blocked public access
5. Pulled a working **bucket policy** from GitHub
6. Applied the public-read policy to allow public access to objects
7. ✅ Successfully accessed the image via URL

---


## 💡 Real-World Tips & Best Practices:

🔐 Avoid public buckets unless absolutely required

✅ Use IAM roles and bucket policies for access control

💾 Enable versioning to protect against accidental deletion

📉 Use lifecycle rules to archive or delete unused objects

🪪 Enable default encryption (SSE-S3 or SSE-KMS)

🧪 Test access with anonymous browser sessions 
---
## 🔗 Resources
📄 Amazon S3 Documentation : https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html

📝 GitHub Gist - Bucket Policy Used :  https://github.com/iam-arunfiddler/AWS-Zero-to-Hero/blob/main/Day%206/Sample%20Bucket%20Policies/AllPublicAccess.json

---

 🎥 [YouTube - Tech by Arun Fiddler](https://www.youtube.com/@TechbyArunFiddler)
 
 💼 [LinkedIn - Arun Fiddler](https://www.linkedin.com/in/arunfiddler)



Happy Learning! 🙌
#AWS #S3 #TamilTutorial #CloudComputing #ArunFiddler #TechbyArunFiddler #DevOps #Tamil
