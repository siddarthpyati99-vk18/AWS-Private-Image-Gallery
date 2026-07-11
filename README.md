# AWS Private Image Gallery

A beginner AWS cloud project that demonstrates how to securely host a private image gallery using Amazon S3, IAM Roles, Amazon EC2, AWS CLI, and Apache Web Server.

---

## Project Overview

This project stores images in a **private Amazon S3 bucket**. An **Amazon EC2** instance securely accesses the bucket using an **IAM Role** (without storing AWS access keys) and hosts a static image gallery through the Apache web server.

---

## AWS Services Used

- Amazon S3 (Private Bucket)
- Amazon EC2 (Amazon Linux 2023)
- IAM Role
- AWS CLI
- Apache HTTP Server

---

## Architecture

```text
                +----------------------+
                |   Amazon S3 Bucket   |
                | (Private Images)     |
                +----------+-----------+
                           |
                    IAM Role (Read Only)
                           |
                           v
                +----------------------+
                | Amazon EC2           |
                | Amazon Linux 2023    |
                | Apache Web Server    |
                +----------+-----------+
                           |
                           v
                    Web Browser
```

---

## Features

- Private S3 bucket for secure image storage
- IAM Role used instead of access keys
- Apache web server hosting the gallery
- Images displayed through a browser
- Beginner-friendly AWS architecture

---

## Project Structure

```
AWS-Private-Image-Gallery/
│
├── index.html
├── images/
│   ├── image1.jpg
│   ├── image2.jpg
│   ├── image3.jpg
│   └── image4.jpg
└── README.md
```

---

## How to Run

1. Launch an Amazon Linux 2023 EC2 instance.
2. Attach an IAM Role with S3 Read access.
3. Install Apache.
4. Copy the website files to `/var/www/html`.
5. Start Apache.
6. Open the EC2 public IP in a browser.

---

## Skills Demonstrated

- Amazon S3
- Amazon EC2
- IAM Roles
- AWS CLI
- Apache Web Server
- Git & GitHub

---

## Future Improvements

- Python Flask
- boto3 integration
- Dynamic image loading
- Multi-AZ deployment
- Application Load Balancer
- Auto Scaling

---

## Author

**Siddarth Pyati**