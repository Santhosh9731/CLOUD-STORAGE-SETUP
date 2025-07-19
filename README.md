# CLOUD-STORAGE-SETUP

*COMPANY* : CODTECH IT SOLUTION

*NAME* : SANTHOSH GOVINDAN

*INTERN ID* : CT06DG1559

*DOMAIN* : CLOUD COMPUTING

*DURATION* : 6 WEEKS

*MENTOR* : NEELA SANTOSH

#### Cloud Storage Task – Amazon S3 Bucket Setup and File Hosting

###  Task Overview

As part of my **Cloud Computing Internship**, I successfully completed a hands-on task involving **Amazon S3**, demonstrating my practical skills in setting up secure and accessible cloud storage solutions. The objective of this task was to create an **S3 bucket**, upload files, configure permissions, and validate public access to hosted objects.

---

###  Steps Completed

  **Bucket Creation:**
I started by creating an S3 bucket named `codtech-storage-demo` in the **EU-North-1 (Stockholm)** region. Amazon S3 buckets act as containers for storing objects such as HTML files, images, or other static content.

 **Uploading Files:**
Next, I uploaded two files to the bucket:

* `website.html` – a simple HTML page demonstrating static website hosting.
* `instance dashboard.png` – an image file showcasing an EC2 instance dashboard.
  The upload process was completed using the AWS S3 console, ensuring both files were correctly listed and their metadata (size, type) verified.

 **Setting Permissions:**
To make the uploaded files publicly accessible, I configured the bucket policy with appropriate permissions. Using a JSON policy, I allowed the `s3:GetObject` action for all users (`Principal: "*"`) on all objects inside the bucket (`Resource: arn:aws:s3:::codtech-storage-demo/*`).
This ensures that anyone with the object URL can view or download the files, which is essential for static website hosting and content delivery.

```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "Statement1",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::codtech-storage-demo/*"
        }
    ]
}
```

 **Testing Access:**
After applying the policy, I validated the public accessibility by directly opening the object URLs in a web browser. The image (`instance dashboard.png`) and the HTML page (`website.html`) were accessible without any authentication, confirming that the permissions were correctly configured.

 **Verification:**
Screenshots were taken at various stages, including the upload window, successful upload summary, final object list, and the bucket policy editor with the green confirmation status indicating a valid policy.
Additionally, a test was conducted by accessing the **EC2 dashboard screenshot** through the public S3 object URL, ensuring that the file hosted on S3 served its purpose.

---

###  Key Skills Demonstrated

✔️ **AWS S3 Management:** Hands-on experience in creating buckets, uploading files, and managing storage resources.
✔️ **Access Control:** Proficiency in writing and applying JSON bucket policies to enable secure yet public access.
✔️ **Static Content Hosting:** Understanding the fundamentals of using S3 as a static file server.
✔️ **AWS Console Navigation:** Confident navigation through AWS services including EC2, IAM, and S3.

---

### 🔗 Conclusion

This task helped reinforce my practical knowledge of **cloud storage concepts**, object permissions, and static content delivery via Amazon S3. I also gained more confidence in using **AWS IAM policies** to manage access securely and efficiently.

Successfully completing this task has given me a solid foundation for future projects involving **website hosting**, **backup storage**, and **cloud-native applications** that leverage S3 for cost-effective and scalable storage.

---

** Repo Purpose:**
This repository serves as a portfolio showcase for my cloud skills. All relevant screenshots, configuration files, and results are included for reference. Feel free to explore and learn!

### OUTPUT

<img width="959" height="505" alt="Image" src="https://github.com/user-attachments/assets/0252259b-9fcd-4558-a82d-3be6c02fe57a" />

