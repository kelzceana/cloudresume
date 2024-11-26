# Cloud Resume Project

This project showcases a cloud-hosted resume built using AWS services and automated deployment pipelines. It highlights cloud technologies and DevOps practices to manage and maintain a professional resume.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Technologies Used](#technologies-used)
- [Project Setup](#project-setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

The Cloud Resume Project is a serverless application that hosts a resume as a static website. It demonstrates the following cloud and DevOps practices:

- Hosting static HTML content on **AWS S3**.
- Using **CloudFront** as a content delivery network (CDN) for improved performance and security.
- Configuring a custom domain with **Route 53**.
- Implementing **CI/CD pipelines** with **GitHub Actions** for automated deployments.

---

## Features

- **Static Hosting**: Resume content is stored and served from an S3 bucket.
- **Global Availability**: CloudFront ensures fast content delivery worldwide.
- **Custom Domain**: The website is accessible via a domain managed in Route 53.
- **SSL/TLS Security**: Secures the website using AWS Certificate Manager for HTTPS.
- **Continuous Deployment**: Updates are automatically deployed using GitHub Actions.

---

## Architecture

[Browser] --> [CloudFront] --> [S3 Bucket] --> [Route 53 for DNS Management]


1. **S3 Bucket**: Stores the static HTML files for the resume.
2. **CloudFront**: Acts as a CDN to deliver content securely and quickly.
3. **Route 53**: Handles the custom domain and DNS records.
4. **GitHub Actions**: Automates updates to the S3 bucket and invalidates the CloudFront cache to reflect changes instantly.

---

## Technologies Used

- **HTML/CSS**: For the static resume content.
- **AWS S3**: To host the static website.
- **AWS CloudFront**: For caching and content delivery.
- **AWS Route 53**: For custom domain management.
- **GitHub Actions**: For CI/CD workflows.
- **AWS Certificate Manager (ACM)**: For SSL/TLS certificates.

---

## Usage
View the Resume: Access the resume via the custom domain configured in Route 53 www.kelechiedeh.info.
