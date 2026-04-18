
Mike's Macaroon Market: Full-Stack AWS Deployment

This repository represents a full-stack cloud migration and infrastructure orchestration project. Originally forked to isolate development, this application was successfully transitioned from a local environment to a scalable, multi-tier architecture on **Amazon Web Services (AWS)**.

🏗️ Architecture Overview

The deployment leverages a "decoupled" architecture to ensure high availability and performance:

* Compute: Node.js application hosted on **Amazon EC2** (Ubuntu/Amazon Linux).
* Database:Persistent data managed via **Amazon RDS** (MySQL/PostgreSQL), connected through secure endpoints.
* Storage:Static assets and product images offloaded to **Amazon S3** to reduce web server load.
* Security:Traffic managed via custom **AWS Security Groups** (Port 8080) and granular **S3 Bucket Policies**.

🚀 DevOps Workflow

1. Source Control & Forking
To maintain a professional deployment lifecycle, the project began with a **GitHub Fork**. 
* Isolated Environment: Forking allowed for custom infrastructure scripting without affecting the upstream source.
* Remote Management:Configured `origin` for personal development and `upstream` for synchronization with the base application.


 🧁 Mike's Macaroon Market: Full-Stack AWS Deployment

This repository represents a full-stack cloud migration and infrastructure orchestration project. Originally forked to isolate development, this application was successfully transitioned from a local environment to a scalable, multi-tier architecture on **Amazon Web Services (AWS)**.

 🏗️ Architecture Overview

The deployment leverages a "decoupled" architecture to ensure high availability and performance:

* Compute: Node.js application hosted on Amazon EC2 (Ubuntu/Amazon Linux).
* Database: Persistent data managed via Amazon RDS (MySQL/PostgreSQL), connected through secure endpoints.
* Storage: Static assets and product images offloaded to **Amazon S3** to reduce web server load.
* Security: Traffic managed via custom **AWS Security Groups** (Port 8080) and granular S3 Bucket Policies.

🚀 DevOps Workflow

1. Source Control & Forking
To maintain a professional deployment lifecycle, the project began with a GitHub Fork. 
Isolated Environment: Forking allowed for custom infrastructure scripting without affecting the upstream source.
Remote Management: Configured `origin` for personal development and `upstream` for synchronization with the base application.

2. Infrastructure Automation

Used Bash scripting to verify and document the environment status. 
Key Tool: `check_git.sh` – A custom script used to audit remote configurations and commit history directly from the CLI.

3. Cloud Integration

Decoupled Storage: Moved hardcoded image paths to S3 Bucket URLs.
Environment Security:
Utilized environment variables to manage database credentials, preventing sensitive data from being committed to version control.

🛠️ Tech Stack

* Cloud: AWS (EC2, S3, RDS)
* Scripting: Bash (Linux/Unix CLI)
* Backend: Node.js
* Version Control: Git / GitHub

 📈 Performance & Cost Optimization

The project was managed within a strict budget, utilizing AWS Credits and t2.micro instances to demonstrate cost-conscious engineering—a vital skill for modern Cloud Support and DevOps roles.


Developed as part of a Cloud Engineering deep-dive to transition from Support to Infrastructure Orchestration.
