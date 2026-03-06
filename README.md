# 🚀 IT Infrastructure Engineer – Complete Roadmap

## 🔰 What is an IT Infrastructure Engineer?

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

## 3 On-prem server knowledge (must-have)
- Server hardware: CPU, RAM, RAID levels
- Storage: SSD (SATA vs NVMe)
- Server management: iDRAC / iLO
- Capacity planning & hardware troubleshooting

## 4 Web servers
	• Apache, Nginx
	• IIS (Windows environments)
	• SSL, reverse proxy, basic performance tuning

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

## 🔹 Windows Server Basics

- Windows Server installation & configuration
- Roles & Features management
- Remote Desktop (RDP) management
- File Server setup
- Printer Server setup

## 🔹 Active Directory (AD DS)

### Core Components

- Domain
- Domain Controller
- Organizational Unit (OU)
- Users & Groups

📌 Example structure

```
company.local
   ├── Sales OU
   ├── IT OU
   └── HR OU
```

## 🔹 User & Group Management

- Create users
- Create groups
- Assign permissions
- Group Policy basics

📌 Example

```
User → IT Department
Group → IT_Admin
Permission → Server access
```

## 🔹 Group Policy (GPO)

Used for **centralized management of computers**

Examples

- Password policy
- Software restriction
- USB control
- Desktop settings

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

# 🧪 PHASE 5 – Storage, Backup & DR Concepts

## 🔹 Storage Types

1️⃣ **DAS (Direct Attached Storage)**

Server connected storage

2️⃣ **NAS (Network Attached Storage)**

File storage over network

3️⃣ **SAN (Storage Area Network)**

High-speed enterprise storage

---

## 🔹 RAID (Very common interview topic)

| RAID | Purpose |
| --- | --- |
| RAID 0 | Performance |
| RAID 1 | Mirroring |
| RAID 5 | Balance |
| RAID 10 | Performance + Redundancy |

---

## 🔹 Backup Types

1️⃣ Full Backup

2️⃣ Incremental Backup

3️⃣ Differential Backup

Example flow

```
Day 1 → Full backup
Day 2 → Incremental
Day 3 → Incremental
```

---

## 🔹 Disaster Recovery (DR)

Concepts for **system failure recovery**

Key elements

- Backup strategy
- Offsite backup
- Recovery testing
- Failover systems

---

## 🔹 Important Metrics

| Metric | Meaning |
| --- | --- |
| RTO | Recovery Time Objective |
| RPO | Recovery Point Objective |

Example

```
RTO = 2 hours
RPO = 30 minutes
```

# 🔐 PHASE 6 – Virtualization & Containers (VMware, Docker, K8s Basics)

## 🔹 Virtualization Concepts

- Virtual Machines (VM)
- Hypervisor (ESXi, Hyper-V)
- Resource allocation (CPU / RAM / Storage)
- VM creation & management

📌 Example

```
Physical Server
   │
Hypervisor
   ├── VM (Linux)
   ├── VM (Windows Server)
   └── VM (Database)
```

---

## 🔹 VMware Basics (Enterprise Standard)

- ESXi installation
- vCenter management
- VM snapshots
- VM cloning
- VM migration (vMotion)
- Resource pools

---

## 🔹 Virtual Networking

- Virtual Switch (vSwitch)
- Port Groups
- VLAN basics

Example

```
VM → vSwitch → Physical Network
```

---

## 🔹 Docker (Container Basics)

- Docker installation
- Images & Containers
- Docker Hub / Registry
- Container networking

📌 Commands

```bash
docker run nginx
docker ps
docker stop container_id
docker images
```

---

## 🔹 Kubernetes Basics

- Cluster
- Node
- Pod
- Deployment
- Service

Example structure

```
Cluster
   ├── Node
   │     └── Pods
   │          └── Containers
```

---

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
## 🔹 VPN & firewall concepts
	• Site-to-site vs remote VPN
	• Firewall rules, NAT, port forwarding
	• Security boundaries and traffic flow


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

## 🔹 Version Control

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
