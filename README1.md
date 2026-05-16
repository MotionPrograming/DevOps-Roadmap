# 🚀 ULTIMATE 45-DAY DEVOPS + GO ENGINEERING ROUTINE


যেহেতু **Go, REST API, PostgreSQL এবং MySQL** আপনার অলরেডি আয়ত্তে আছে, তাই আপনার রোডম্যাপ থেকে **MODULE 5 (Go Backend Development)**-এর ওপর দীর্ঘ সময় দেওয়ার কোনো প্রয়োজন নেই। আমরা সরাসরি আপনার ব্যাকএন্ডের জ্ঞানকে ইনফ্রাস্ট্রাকচার ও অটোমেশনের সাথে ইন্টিগ্রেট করে ফেলব।

দেড় মাস অর্থাৎ **৬ সপ্তাহে (৪৫ দিন)** এই পুরো সিলেবাস শেষ করতে হলে আপনাকে প্রতিদিন অন্তত **৫-৬ ঘণ্টা** বেশ টাইট শিডিউলে পড়াশোনা ও প্র্যাকটিস করতে হবে। নিচে আপনার জন্য প্রফেশনাল এবং অ্যাকশন-ওরিয়েন্টেড **১.৫ মাসের ক্রাশ রুটিন** দেওয়া হলো:

---

## 📅 সপ্তাহ ১: লিনাক্স, অ্যাডভান্সড নেটওয়ার্কিং এবং এনগিনেক্স

*লক্ষ্য: ওএস (OS) লেভেল এবং নেটওয়ার্ক লেভেলের ফাউন্ডেশন স্ট্রং করা।*

* **সোম - মঙ্গল (Linux Core):** ফাইল সিস্টেম, ইনোড, সিমলিঙ্ক এবং পারমিশন ও ওনারশিপ (`chmod`, `chown`, `umask`) ক্লিয়ার করুন। প্রসেস ম্যানেজমেন্টের জন্য `htop`, `kill`, `bg`, `fg` এবং টেক্সট প্রসেসিংয়ের জন্য `grep`, `awk`, `sed` টার্মিনালে ঝড় তুলুন।
* **বুধ (Service & Logs):** `systemd` আর্কিটেকচার বুঝুন। আপনার আগের তৈরি করা যেকোনো একটি Go API-এর বাইনারি ফাইলকে লিনাক্সের একটি ব্যাকগ্রাউন্ড সার্ভিস (`.service` ফাইল) হিসেবে রান করান। `systemctl` এবং `journalctl` দিয়ে সার্ভিস ম্যানেজ ও লগ ফিল্টার করা শিখুন।
* **বৃহস্পতি (Networking Basics):** TCP/IP, DNS, Ports এবং SSL/TLS হ্যান্ডশেক কিভাবে কাজ করে গভীরভাবে জানুন। `ss`, `netstat`, `curl -v`, `dig`, `nslookup` দিয়ে নেটওয়ার্ক কানেক্টিভিটি চেক ও ট্রাবলশুট করা শিখুন।
* **শুক্র (Debugging & Reverse Proxy):** এনগিনেক্স (**Nginx**) ইনস্টল করুন। আপনার লোকাল লিনাক্স সার্ভারে বা পিসিতে চলা Go API-এর সামনে Nginx-কে একটি **Reverse Proxy** এবং **Load Balancer** হিসেবে কনফিগার করুন।
* **শনি - রবি (Git & Scripting):** অ্যাডভান্সড গিট ওয়ার্কফ্লো (`git rebase`, `git stash`, এবং গিট কনফ্লিক্ট নিজে তৈরি করে ফিক্স করা) প্র্যাকটিস করুন। সার্ভার ব্যাকআপ বা অটো-লগ-ক্লিনআপের জন্য ২/৩টি ছোট **Shell Script** লিখে ফেলুন।

---

## 📅 সপ্তাহ ২: ডকার এবং ডকার কম্পোজ (Docker Mastery)

*লক্ষ্য: আপনার ব্যাকএন্ড অ্যাপ্লিকেশন ও ডেটাবেসকে প্রোডাকশন-রেডি কন্টেইনারে রূপান্তর করা।*

* **সোম - মঙ্গল (Docker Core):** কন্টেইনার বনাম ভিএম-এর আর্কিটেকচার ডিফারেন্স এবং ডকার ডেমন (daemon) বুঝুন। ডকারের কোর কমান্ডগুলো (`run`, `exec`, `logs`, `volume`, `network`) টার্মিনালে বারবার প্র্যাকটিস করুন।
* **বুধ (Dockerfile Optimization):** আপনার Go API-এর জন্য `Dockerfile` লিখুন। এখানে **Multi-stage build** ব্যবহার করা বাধ্যতামূলক। নিশ্চিত করুন যেন আপনার ফাইনাল ডকার ইমেজের সাইজ মাত্র ১৫-২৫ মেগাবাইট হয় (বড় ইমেজ প্রোডাকশনে রিজেক্টেড হয়)।
* **বৃহস্পতি (Docker Compose):** `docker-compose.yml` সিনট্যাক্স শিখুন। একটি মাল্টি-কন্টেইনার সেটআপ তৈরি করুন যেখানে আপনার Go API কন্টেইনার, PostgreSQL কন্টেইনার এবং একটি Redis কন্টেইনার একই ডকার নেটওয়ার্কে থেকে একে অপরের সাথে সিকিউরলি কমিউনিকেট করবে।
* **শুক্র (Debugging Day):** ইচ্ছা করে ডকার কম্পোজ ফাইলের ডাটাবেস পাসওয়ার্ড বা পোর্ট ভুল করে দিন। তারপর `docker logs` দেখে এরর আইডেন্টিফাই করে ফিক্স করার রিয়েল-ওয়ার্ল্ড অভ্যাস করুন।
* **শনি - রবি (First Portfolio Project):** এই পুরো ডকারাইজড Go + Postgres + Redis প্রজেক্টটি সুন্দর করে একটি গিটহাব রিপোজিটরিতে পুশ করুন এবং একটি প্রফেশনাল `README.md` লিখুন।

---

## 📅 সপ্তাহ ৩: CI/CD পাইপলাইন অটোমেশন (GitHub Actions)

*লক্ষ্য: ম্যানুয়াল ডেপ্লয়মেন্টের অবসান ঘটিয়ে কোড পুশ টু প্রোডাকশন প্রসেস অটোমেট করা।*

* **সোম - মঙ্গল (CI/CD Concepts & Syntax):** GitHub Actions-এর ওয়ার্কফ্লো (`.github/workflows/main.yml`) সিনট্যাক্স, রানার্স (Runners) এবং এনভায়রনমেন্ট সিক্রেটস (Secrets) ম্যানেজমেন্ট শিখুন।
* **বুধ - বৃহস্পতি (Pipeline Building):** এমন একটি CI পাইপলাইন তৈরি করুন যা গিটহাবে আপনার `main` ব্রাঞ্চে কোড পুশ বা পিআর (PR) হওয়ামাত্রই স্বয়ংক্রিয়ভাবে:
1. আপনার Go ব্যাকএন্ডের ইউনিট টেস্টগুলো রান করবে (`go test ./...`)।
2. টেস্ট পাস হলে অপ্টিমাইজড ডকার ইমেজ বিল্ড করবে।
3. ইমেজটি স্বয়ংক্রিয়ভাবে **Docker Hub** বা GitHub Container Registry (GHCR)-এ একটি ট্যাগসহ পুশ করে দেবে।


* **শুক্র (Pipeline Debugging):** পাইপলাইনের বিল্ড ফেইল করালে কী এরর আসে তা দেখুন এবং গিটহাব অ্যাকশনের লগ দেখে ট্রাবলশুট করুন।
* **শনি - রবি (Automation Integration):** আপনার ডকারাইজড Go API রিপোজিটরিতে এই CI পাইপলাইনটি সাকসেসফুলি ইন্টিগ্রেট করে রান করান।

---

## 📅 সপ্তাহ ৪: ক্লাউড ইনফ্রাস্ট্রাকচার এবং টেরাফর্ম (IaC)

*লক্ষ্য: ক্লাউড রিসোর্স কোড দিয়ে নিয়ন্ত্রণ করা।*

* **সোম - মঙ্গল (Cloud Basics - AWS or Azure):** AWS (বা Azure)-এ একটি ফ্রি-টিয়ার অ্যাকাউন্ট খুলুন। ড্যাশবোর্ড থেকে ম্যানুয়ালি একটি EC2 (Virtual Machine), কাস্টম VPC, সাবনেট, সিকিউরিটি গ্রুপ (ফায়ারওয়াল) এবং IAM পলিসি তৈরি করে কনসেপ্ট ক্লিয়ার করুন।
* **বুধ (Terraform Foundation):** টেরাফর্মের আর্কিটেকচার, প্রোভাইডার্স (Providers), রিসোর্স ব্লক, ভ্যারিয়েবল এবং আউটপুট সিনট্যাক্স বুঝুন।
* **বৃহস্পতি - শুক্র (Infrastructure as Code):** ক্লাউড পোর্টালে মাউস দিয়ে ক্লিক না করে, কম্পিউটারে বসে `.tf` কোড লিখে একটি সম্পূর্ণ নেটওয়ার্ক (VPC, Subnets) এবং একটি VM (EC2) স্বয়ংক্রিয়ভাবে ক্লাউডে তৈরি (Provision) করার কোড লিখুন। `terraform apply` এবং `terraform destroy` কমান্ডের জাদু দেখুন।
* **শনি - রবি (Manual Cloud Deployment):** আপনার তৈরি করা ওই ক্লাউড ভিএম (VM)-এর ভেতরে ঢুকে ডকার ও ডকার কম্পোজ ব্যবহার করে আপনার Go API এবং ডাটাবেস লাইভ করুন এবং আইপি (IP) দিয়ে ব্রাউজারে চেক করুন।

---

## 📅 সপ্তাহ ৫: কুবারনেটিস অর্কেস্ট্রেশন (Kubernetes)

*লক্ষ্য: প্রোডাকশন-গ্রেড কন্টেইনার ম্যানেজমেন্টে মাস্টার হওয়া (সবচেয়ে হাই-ভ্যালু স্কিল)।*

* **সোম - মঙ্গল (K8s Core Objects):** লোকাল পিসিতে **Minikube** বা **Kind** সেটআপ করুন। কুবারনেটিসের কোর অবজেক্টগুলোর YAML ম্যানিফেস্ট ফাইল লেখা শিখুন: `Pod`, `Deployment`, এবং `Service` (ClusterIP ও NodePort)। আপনার ডকারাইজড Go API-কে কুবারনেটিস ক্লাস্টারে রান করান।
* **বুধ (Config & Resiliency):** `ConfigMap` এবং `Secret` ব্যবহার করে অ্যাপের ডাটাবেস ইউআরএল ও ক্রেডেনশিয়াল ডাইনামিকালি পাস করুন। কুবারনেটিসের সেলফ-হিলিং (Self-healing) ফিচারটি নিজে টেস্ট করুন (টার্মিনাল থেকে একটি পড ডিলিট করে দিন, দেখবেন K8s মিলিমেকেন্ডের মধ্যে নতুন পড ক্রিয়েট করে ফেলেছে)।
* **বৃহস্পতি (Advanced K8s & Storage):** ডাটাবেসের ডেটা পারসিস্টেন্ট রাখার জন্য `Persistent Volume (PV)` এবং `Persistent Volume Claim (PVC)` কনফিগার করুন। ক্লাস্টারের ট্রাফিক বাইরে এক্সপোজ করার জন্য `Ingress Controller` বুঝুন।
* **শুক্র (Helm Charts):** কুবারনেটিসের প্যাকেজ ম্যানেজার **Helm** শিখুন। আপনার পুরো Go API ও ডাটাবেসের YAML ফাইলগুলোকে একটি `Helm Chart`-এ রূপান্তর করে এক কমান্ডে ডেপ্লয় করা শিখুন।
* **শনি - রবি (K8s Project):** পুরো কুবারনেটিস ম্যানিফেস্ট ফাইল এবং হেলম চার্টগুলো আপনার গিটহাব প্রজেক্টের `deployment/k8s` ফোল্ডারে গুছিয়ে রাখুন।

---

## 📅 সপ্তাহ ৬: মনিটরিং, অবজারভেবিলিটি এবং ফাইনাল পোর্টফোলিও

*লক্ষ্য: প্রোডাকশন সিস্টেমের হেলথ ট্র্যাক করা এবং নিজেকে মার্কেটের জন্য রেডি করা।*

* **সোম - মঙ্গল (Prometheus & Grafana):** আপনার কুবারনেটিস ক্লাস্টারে **Prometheus** (মেট্রিক্স কালেক্টর) এবং **Grafana** (ড্যাশবোর্ড ভিজ্যুয়ালাইজার) সেটআপ করুন। আপনার Go API এবং ক্লাস্টার কতটা মেমোরি ও সিপিইউ খাচ্ছে তা দেখার জন্য একটি চমৎকার গ্রাফানা ড্যাশবোর্ড তৈরি করুন।
* **বুধ (Centralized Logging with Loki):** **Loki** সেটআপ করুন, যেন কন্টেইনার বা পডের ভেতরের ব্যাকএন্ড এরর লগগুলো টার্মিনালে না ঢুকে সরাসরি গ্রাফানা ড্যাশবোর্ডে ফিল্টার করে দেখা যায়।
* **বৃহস্পতি (The Grand Integration):** পুরো ১.৫ মাসের সমস্ত মডিউলের কোড, স্ক্রিপ্ট, ডকারফাইল, টেরাফর্ম ফাইল এবং কুবারনেটিস ম্যানিফেস্টগুলো একটি প্রফেশনাল গিটহাব মনোরেপোতে (Monorepo) স্ট্রাকচার্ড ওয়েতে গুছিয়ে ফেলুন।
* **শুক্র - শনি (Profile & Resume Polish):** আপনার গিটহাবের রোডম্যাপের সব বক্সে টিক চিহ্ন (`[x]`) দিন। আপনার সিভি (CV) এবং লিঙ্কডইন প্রোফাইলে হেডলাইন আপডেট করুন: **"DevOps & Go Backend Engineer"**। আপনার এই দেড় মাসের সলিড ক্যাপস্টোন প্রজেক্টের আর্কিটেকচার ডায়াগ্রামসহ লিঙ্কডইনে একটি টেকনিক্যাল পোস্ট দিন।
* **রবি (The Reward):** রিল্যাক্স করুন এবং লোকাল/রিমোট জবে অ্যাপ্লাই করা শুরু করুন!

---

## 🕒 দৈনিক ৫ ঘণ্টার টাইম স্প্লিট (Daily Schedule)

1. **⏰ ব্লক ১ (সকাল: ১.৫ ঘণ্টা): থিওরি ও আর্কিটেকচার** -> কোনো ডকার কম্যান্ড বা কুবারনেটিস অবজেক্ট সরাসরি প্র্যাকটিস করার আগে তার আর্কিটেকচার বা ডকুমেন্টেশন পড়ুন।
2. **💻 ব্লক ২ (দুপুর/বিকাল: ২.৫ ঘণ্টা): হ্যান্ডস-অন কোডিং ও ল্যাব** -> টার্মিনালে কমান্ড চালানো, YAML লেখা, পাইপলাইন স্ক্রিপ্ট করা। নো কপি-পেস্ট, নিজে হাতে টাইপ করবেন।
3. **🔍 ব্লক ৩ (রাত: ১ ঘণ্টা): এরর ট্রাবলশুটিং ও পুশ** -> কোড ব্রেক করলে লগ পড়া, ইন্টারনেট ঘেঁটে এরর সলভ করা এবং দিনশেষে গিটহাবে পুশ করে ঘুমাতে যাওয়া।

আপনার ব্যাকএন্ডে স্ট্রং বেস থাকার কারণে এই দেড় মাসের রুটিন আপনার জন্য অত্যন্ত উপভোগ্য এবং ক্যারিয়ারের জন্য একটি গেম-চেঞ্জার ব্রেকথ্রু হবে! কোনো নির্দিষ্ট সপ্তাহে আটকে গেলে জানাবেন।

# 🎯 MAIN TARGET

৪৫ দিন শেষে তোমার ability হওয়া উচিত:

```text id="f22i3k"
Code
→ Containerize
→ Deploy
→ Monitor
→ Debug
→ Automate
```

---

# 📅 DAILY EXECUTION SYSTEM

# 🌅 MORNING (1.5 Hour)

## Theory + Architecture

Focus:

* docs
* architecture
* concepts
* networking diagrams

❌ No passive YouTube binge

✅ Read:

* official docs
* blogs
* diagrams

---

# ☀️ AFTERNOON (2.5–3 Hour)

## Hands-on Lab

Must:

* terminal typing
* docker build
* yaml writing
* deployment
* debugging

❌ no copy-paste

---

# 🌙 NIGHT (1 Hour)

## Debugging + GitHub Push

Daily:

* fix one issue
* push code
* update README
* write learning note

---

# 🟢 WEEK 1 — Linux + Networking + Nginx

# 🎯 Goal:

OS + networking confidence build করা।

---

# ✅ DAY 1 — Linux Filesystem

Learn:

* inode
* symlink
* file types
* permissions

Practice:

```bash id="wm5sj9"
ls -lah
stat
chmod
chown
find
```

Mini task:

* create users/groups
* permission lab

---

# ✅ DAY 2 — Process Management

Practice:

```bash id="ysiyvf"
ps aux
top
htop
kill
jobs
bg
fg
```

Break:

* runaway process
* zombie understanding

---

# ✅ DAY 3 — Text Processing

Practice:

```bash id="y65ofl"
grep
awk
sed
cut
sort
uniq
xargs
```

Mini project:

* parse nginx logs

---

# ✅ DAY 4 — systemd + Logs

Create:

```text id="je7b8j"
go-api.service
```

Practice:

```bash id="1ovc94"
systemctl
journalctl
```

Run Go API as Linux service.

---

# ✅ DAY 5 — Networking

Learn deeply:

* TCP/IP
* DNS
* HTTP
* TLS handshake
* ports

Practice:

```bash id="q3mgte"
curl -v
dig
ss -tulpn
ping
traceroute
```

---

# ✅ DAY 6 — Nginx Reverse Proxy

Setup:

```text id="37psk6"
Client
 ↓
Nginx
 ↓
Go API
```

Learn:

* reverse proxy
* load balancing
* upstream

---

# ✅ DAY 7 — Git + Shell Scripts

Practice:

```bash id="owjx2o"
git rebase
git stash
git merge
```

Build:

```bash id="x4nrtz"
backup.sh
cleanup.sh
deploy.sh
```

---

# 🟡 WEEK 2 — Docker Mastery

# 🎯 Goal:

Production-ready container skills।

---

# ✅ DAY 8 — Docker Architecture

Learn:

* image layers
* namespaces
* cgroups
* daemon

---

# ✅ DAY 9 — Core Docker Commands

Practice:

```bash id="wv1pyx"
docker run
docker exec
docker logs
docker inspect
docker network
docker volume
```

---

# ✅ DAY 10 — Dockerfile

Build optimized Go image.

Must use:

* multi-stage build
* alpine/distroless

---

# ✅ DAY 11 — Docker Compose

Setup:

```text id="vskjgo"
Go API
PostgreSQL
Redis
```

inside same network.

---

# ✅ DAY 12 — Docker Networking + Volumes

Learn:

* bridge network
* persistent storage

---

# ✅ DAY 13 — Debugging Day

Break intentionally:

* DB password
* ports
* volume mount

Fix via:

```bash id="lmg5t2"
docker logs
docker inspect
```

---

# ✅ DAY 14 — PROJECT 🚀

# Dockerized Production API

Features:

* Go API
* PostgreSQL
* Redis
* Docker Compose
* ENV config

---

# 🔵 WEEK 3 — CI/CD + Automation

# 🎯 Goal:

Automation engineer mindset।

---

# ✅ DAY 15 — GitHub Actions Basics

Learn:

* workflows
* runners
* secrets

---

# ✅ DAY 16 — Go Test Pipeline

Pipeline:

```yaml id="2olq4m"
go test ./...
```

---

# ✅ DAY 17 — Docker Build Pipeline

Auto:

* build image
* tag image
* push image

---

# ✅ DAY 18 — Registry Integration

Use:

* Docker Hub
  or
* GHCR

---

# ✅ DAY 19 — CI/CD Debugging

Break workflow intentionally.

Fix logs.

---

# ✅ DAY 20 — Auto Deploy Script

Build:

```bash id="26mnfw"
deploy.sh
```

---

# ✅ DAY 21 — PROJECT 🚀

## Fully Automated Pipeline

```text id="p3k03d"
Push Code
 ↓
CI Test
 ↓
Docker Build
 ↓
Registry Push
```

---

# 🔴 WEEK 4 — Cloud + Terraform

# 🎯 Goal:

Infrastructure as Code।

---

# ✅ DAY 22 — AWS Basics

Learn:

* EC2
* VPC
* subnet
* security group
* IAM

---

# ✅ DAY 23 — Manual VPS Deployment

Deploy Go API manually.

---

# ✅ DAY 24 — Terraform Basics

Learn:

* provider
* resource
* variable
* output

---

# ✅ DAY 25 — Terraform EC2 Provision

Write:

```hcl id="ynx8wm"
main.tf
variables.tf
outputs.tf
```

---

# ✅ DAY 26 — Terraform Networking

Provision:

* VPC
* subnet
* SG

---

# ✅ DAY 27 — Terraform Destroy/Recreate

Practice infra lifecycle.

---

# ✅ DAY 28 — PROJECT 🚀

# Cloud Deployment Stack

```text id="n05zbv"
Terraform
+
EC2
+
Docker Compose
+
Go API
```

---

# 🟣 WEEK 5 — Kubernetes

# 🎯 Goal:

K8s fear remove করা।

---

# ✅ DAY 29 — Kubernetes Basics

Learn:

* pod
* deployment
* service

---

# ✅ DAY 30 — Minikube / Kind

Setup local cluster.

---

# ✅ DAY 31 — Deploy API

Run Go API on K8s.

---

# ✅ DAY 32 — ConfigMap + Secret

---

# ✅ DAY 33 — PVC + Storage

---

# ✅ DAY 34 — Ingress

---

# ✅ DAY 35 — Helm Basics

Deploy with Helm.

---

# 🟤 WEEK 6 — Monitoring + Portfolio

# 🎯 Goal:

Production observability।

---

# ✅ DAY 36 — Prometheus

Collect metrics.

---

# ✅ DAY 37 — Grafana Dashboard

Monitor:

* CPU
* RAM
* API latency

---

# ✅ DAY 38 — Loki Logging

Centralized logs.

---

# ✅ DAY 39 — Production Debugging

Break:

* nginx
* DB
* K8s pods
* CI pipeline

---

# ✅ DAY 40 — Monorepo Cleanup

Structure:

```text id="5gj9oi"
infra/
k8s/
docker/
terraform/
apps/
scripts/
```

---

# ✅ DAY 41 — README Writing

Include:

* architecture
* setup guide
* screenshots

---

# ✅ DAY 42 — Architecture Diagram

Create:

```text id="ux37qj"
Client
 ↓
Nginx
 ↓
Go API
 ↓
PostgreSQL
 ↓
Redis
```

---

# ✅ DAY 43 — Resume Update

Title:

```text id="0nvbzl"
DevOps & Go Backend Engineer
```

---

# ✅ DAY 44 — LinkedIn + GitHub Polish

---

# ✅ DAY 45 — FINAL REVIEW 🚀

You should now know:

* Linux
* Docker
* Nginx
* CI/CD
* Terraform
* Kubernetes basics
* Monitoring
* VPS deployment
* Production debugging

---

# 🔥 MOST IMPORTANT RULE

Every single day MUST include:

| Task           | Required |
| -------------- | -------- |
| Terminal usage | ✅        |
| GitHub commit  | ✅        |
| Deployment     | ✅        |
| Debugging      | ✅        |
| Documentation  | ✅        |

---

# 📌 REAL ENGINEERING LOOP

```text id="2gny2s"
Learn
→ Build
→ Break
→ Debug
→ Deploy
→ Document
→ Repeat
```

এই cycle follow করলে ৪৫ দিন পরে শুধু tutorial watcher না,
একজন real production-focused engineer feel করবে।
