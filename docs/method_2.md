# n8n Local Installation Guide (Docker Only)

This guide explains how to install and run **n8n locally on your desktop using Docker**.

All commands are written for **Bash / Terminal / Command Prompt**.

---

# Step 1: Install Docker Desktop

Download and install Docker Desktop from the official website:

https://www.docker.com/

---

# Step 2: Verify Docker Installation

Open your terminal and run:

bash:
docker --version

---

# Step 3: Run n8n Container (Temporary Mode)

Run n8n without saving data permanently:

bash:
docker run -it --rm \
  -p 5678:5678 \
  n8nio/n8n

---

# Step 4: Run n8n with Persistent Data (Recommended)

Run n8n and store data permanently on your system:

bash:
docker run -it --rm \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n


---

# Step 5: Access n8n in Browser

Open your browser and visit:

http://localhost:5678


---

# Step 6: Stop the Container

To stop n8n:

CTRL + C


---
