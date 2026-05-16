# 🚀 ULTIMATE 45-DAY DEVOPS + GO ENGINEERING ROUTINE

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
