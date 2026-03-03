# 🚀 IT Infrastructure Engineer – Complete Roadmap

## 🔰 What is an IT Infrastructure Engineer?

An **IT Infrastructure Engineer** designs, builds, operates, and maintains:

- **Servers**
- **Networks**
- **Operating Systems**
- **Cloud platforms**
- **Security**
- **Monitoring & automation**

In Japan, this role is often called:

- インフラエンジニア
- サーバーエンジニア
- ネットワークエンジニア
- クラウドエンジニア（上位）

---

# 📘 PHASE 1 – IT Basics (ITパスポート, **基本情報技術者試験**)

## 1️⃣ Computer & OS Fundamentals

### 🔹 Types of OS

| OS | Usage |
| --- | --- |
| Windows Server | Corporate environments |
| Linux (Ubuntu, CentOS, RHEL) | Servers, cloud |
| macOS | Dev environment |

### 🔹 Key concepts

- CPU / RAM / Disk
- Kernel vs User space
- Process vs Thread

📌 Example:

```bash
top
ps aux
free -h
df -h

```

---

## 2️⃣ Networking Basics (EXTREMELY IMPORTANT)

### 🔹 Network Types

1. LAN (Local Area Network)
2. WAN (Wide Area Network)
3. VPN (Virtual Private Network)

### 🔹 Core concepts (must memorize)

| Term | Meaning |
| --- | --- |
| IP Address | Device identity |
| Subnet Mask | Network range |
| Gateway | Exit point |
| DNS | Name → IP |
| DHCP | Auto IP assign |

📌 Example:

```
PC → Router → ISP → Internet

```

📌 Commands:

```bash
ip a
ping google.com
traceroute google.com
nslookup google.com

```

---

# 🖥️ PHASE 2 – Linux Server Mastery (LPIC-1)

## 1️⃣ Linux File System

```
/etc  → config files
/var  → logs
/home → users
/bin  → commands

```

## 2️⃣ User & Permission (VERY COMMON INTERVIEW TOPIC)

### 🔹 Permission types

| Type | Symbol |
| --- | --- |
| Read | r |
| Write | w |
| Execute | x |

```bash
chmod 755 file.sh
chown user:group file

```

---

## 3️⃣ Services & Processes

```bash
systemctl start nginx
systemctl status sshd
journalctl -u nginx

```

---

# 🖥️ PHASE 3 – Windows Server & Active Directory

---

# 🌐 PHASE 4 – Networking (CCNA)

## 🔹 Network Device Types

1. Router
2. Switch
3. Firewall
4. Load Balancer

## 🔹 Protocol Classification (Important)

### Application Layer

- HTTP / HTTPS
- FTP / SFTP
- SMTP

### Transport Layer

- TCP (reliable)
- UDP (fast)

📌 Example:

- Web = TCP 443
- DNS = UDP 53

---

# 🧪 PHASE 5 – Storage, Backup & DR concepts

# 🔐 PHASE 6 – Virtualization & Containers (VMware, Docker, K8s basics)

# ☁️ PHASE 7 – Cloud Computing (AWS SAA)

## 🔹 Cloud Types

1. IaaS (AWS EC2)
2. PaaS (Heroku)
3. SaaS (Google Workspace)

## 🔹 AWS Core Services (Japan demand 🔥)

| Service | Use |
| --- | --- |
| EC2 | Virtual server |
| S3 | Storage |
| VPC | Network |
| RDS | Database |
| IAM | Access control |
| Serverless | AWS Lambda |

📌 Example architecture:

```
User → ALB → EC2 → RDS

```

🎯 Target cert:

- **AWS Certified Solutions Architect – Associate**

---

# 🔐 PHASE 8 – Security (**情報セキュリティマネジメント試験**)

## 🔹 Security Types

1. Network Security
2. OS Security
3. Application Security
4. Cloud Security

## 🔹 Common attacks (Interview)

- DDoS
- Brute force
- SQL Injection

📌 Tools:

```bash
ufw
iptables
fail2ban

```

---

# 📊 PHASE 9 – Monitoring & Troubleshooting

## 🔹 Monitoring Tools

- Prometheus
- Grafana
- CloudWatch

## 🔹 Logs

```bash
/var/log/syslog
/var/log/nginx/access.log

```
## 🔹 App Performance Metrics

## 🔹 Load Balancing

📌 Incident flow:

```
Alert → Analyze → Fix → Prevent → Report

```

---

# 🤖 PHASE 10 – Automation & DevOps Basics

## 🔹 Scripting

- Bash
- Python (you already know 👍)

📌 Example:

```bash
#!/bin/bash
df -h > disk_report.txt

```

## 🔹 Infrastructure as Code

- Terraform
- Ansible
- Chef

---

## 🔹 Architecture as Code
- Infra Reverse
- Auto Documentation 
- ArchOps

# 🧪 PHASE 11 – Hands-On Projects (VERY IMPORTANT)

## 🔹 Project Ideas (Do ALL)

1. Linux server setup + SSH hardening
2. Web server (Nginx + SSL)
3. AWS EC2 + S3 + IAM
4. Monitoring dashboard
5. Backup automation script

🎯 Put these on:

- GitHub
- Portfolio PDF (Japanese)

---

# 🇯🇵 PHASE 12 – Japan Job Preparation

## 🔹 Japanese Technical Words

| English | Japanese |
| --- | --- |
| Server | サーバー |
| Network | ネットワーク |
| 장애 | 障害 |
| Log | ログ |
| Operation | 運用 |

## 🔹 JLPT + IT

- N3 → Understand tickets
- N2 → Meetings
- **N1 → Design & explanation**

---

# 📅 PHASE 10 – Timeline (Realistic)

| Time | Level |
| --- | --- |
| 0–3 months | IT basics + Linux |
| 4–6 months | Networking + Security |
| 7–9 months | AWS + Projects |
| 10–12 months | Job ready |

---

# 🎯 Final Career Path

```
Infrastructure Engineer
   ↓
Cloud Engineer
   ↓
Architect / SRE

```

---
