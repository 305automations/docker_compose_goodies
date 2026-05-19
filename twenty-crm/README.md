# Twenty CRM Deployment
Production Ready Self Hosted Twenty CRM Stack

Managed and customized by 305 Automations.

---

# Overview

This repository contains a production ready deployment stack for Twenty CRM using Docker Compose.

The goal is simple:

- Self hosted CRM infrastructure
- Workflow automation
- Centralized lead management
- AI integrations
- Automated outreach systems
- Operational scalability

Because businesses should automate repetitive work instead of paying employees to manually move information between browser tabs like exhausted office librarians from the digital middle ages.

---

# Features

This stack is designed for:

- VPS deployments
- Dedicated servers
- Proxmox environments
- Ubuntu servers
- Docker infrastructure

Included capabilities:

- Twenty CRM
- PostgreSQL
- Redis
- Reverse proxy support
- SSL compatibility
- Automated workflows
- AI integrations
- SMTP email support
- Lead discovery integrations
- Google Maps API workflows

---

# Requirements

Recommended minimum server:

- 4 vCPU
- 8GB RAM
- 80GB SSD
- Ubuntu 24.04 LTS

Required software:

- Docker
- Docker Compose

---

# Installation

## Clone Repository

```bash
git clone https://github.com/YOUR_COMPANY/YOUR_REPOSITORY.git

cd YOUR_REPOSITORY
```

---

## Configure Environment Variables

Copy the example environment file:

```bash
cp .env.example .env
```

Edit the configuration:

```bash
nano .env
```

---

## Generate Secure App Secret

```bash
openssl rand -base64 32
```

Replace:

```env
APP_SECRET=
```

with your generated value.

---

## Start the Stack

```bash
docker compose up -d
```

---

## Verify Containers

```bash
docker compose ps
```

---

# Reverse Proxy

Recommended reverse proxies:

- Traefik
- Nginx Proxy Manager
- Caddy
- Nginx

Make sure SSL is enabled before exposing the instance publicly.

Because exposing unprotected services to the internet is how sysadmins accidentally create educational cybersecurity case studies.

---

# SMTP Configuration

Configure your SMTP provider inside the `.env` file.

Supported providers include:

- Gmail
- Mailgun
- Amazon SES
- SendGrid
- Zoho Mail
- Proton Mail Bridge

SMTP is required for:

- User invitations
- Workflow notifications
- Automated email campaigns
- Password recovery

---

# Workflow Automation

Twenty CRM includes a powerful built in workflow engine.

You can automate:

- Lead assignment
- Follow ups
- Email campaigns
- Webhooks
- AI actions
- Task generation
- Notifications
- Lead enrichment
- Pipeline updates

At 305 Automations, we also build custom workflow systems for businesses using:

- Google Maps API
- Automated lead discovery
- Website scraping
- Contact enrichment
- AI assisted workflows
- Automated outreach systems

---

# Automated Lead Discovery

Our custom automation systems can:

- Search businesses by ZIP code
- Search by niche or industry
- Collect business websites
- Gather phone numbers
- Discover public email addresses
- Extract social media profiles
- Automatically populate Twenty CRM

Examples:

- Roofing companies in Miami
- Dental clinics in Orlando
- Beauty salons in Pinecrest
- Marble companies in South Florida

The entire process becomes centralized and automated.

No spreadsheets.
No manual searching.
No employees opening 42 browser tabs while silently reconsidering their career choices.

---


# Backup Recommendations

Recommended backup strategy:

- Daily PostgreSQL dumps
- Offsite backups
- Weekly Docker volume snapshots
- Automated restore testing

Because backups are only theoretical until someone actually restores them successfully.

---

# Security Recommendations

Recommended production security:

- Enable SSL
- Use strong passwords
- Restrict server ports
- Enable firewall rules
- Keep Docker updated
- Use fail2ban
- Enable automatic backups

---

# Maintenance

Useful commands:

## View Logs

```bash
docker compose logs -f
```

## Restart Services

```bash
docker compose restart
```

## Stop Stack

```bash
docker compose down
```

## Update Containers

```bash
docker compose pull

docker compose up -d
```

---

# Services by 305 Automations

We help businesses deploy and automate Twenty CRM environments tailored to their operations.

Services include:

- Infrastructure deployment
- Docker setup
- Workflow automation
- Lead generation systems
- Automated outreach
- AI integrations
- API integrations
- VPS hardening
- Reverse proxy setup
- Maintenance and support

Website:

https://305automations.com

---

# License

Review the official Twenty CRM licensing and terms before commercial deployment.

Official Twenty CRM Website:

https://twenty.com

Official Documentation:

https://docs.twenty.com