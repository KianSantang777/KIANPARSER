# Dork Parser by Kiansantang Dev

<p align="center">
  <img src="https://raw.githubusercontent.com/KianSantang777/KIANPARSER/refs/heads/main/dorkparser.png" width="720" alt="Dork Parser Preview">
</p>

**Dork Parser** is an automated tool designed to extract and collect URLs from various search engines using custom search queries known as **dorks**.

It intelligently filters the results, removing irrelevant or duplicate links, and saves only valid, usable URLs.  
This tool is useful for information gathering, penetration testing, or search-based data scraping.

---

## Key Features

- Supports multiple search engines: Google, Bing, Yahoo, Yandex, DuckDuckGo, Brave, and more.
- Proxy support (HTTP, SOCKS4/5) to bypass rate limits and improve anonymity.
- Smart filtering to remove known domains, redirects, unwanted paths, and duplicates.
- Real-time statistics (requests per minute, valid URLs, errors, retries, etc.).
- Automatically saves results into the `results/` folder with timestamps.

## How to Install

This tool requires **Python 3.12+** and a few Python packages.  
Below are the installation steps for **Termux** (Android) and **Ubuntu/Linux**.

---

### On Termux (Android)

```bash
# Update and upgrade packages
pkg update && pkg upgrade

# Install Python and dependencies
pkg install python git openssl clang libxml2 libxslt -y

# Optional: upgrade pip
pip install --upgrade pip

# Clone the repository
git clone https://github.com/KianSantang777/KIANPARSER

# Change directory
cd KIANPARSER

# Install Python requirements
pip install -r requirements.txt

# Run the tool
python dorkparser.py
```
### On Ubuntu / Debian-based Systems
```
# Update system packages
sudo apt update && sudo apt upgrade -y

# Install Python 3.12 and required packages
sudo apt install python3 python3-pip git build-essential libssl-dev libxml2-dev libxslt1-dev -y

# Optional: upgrade pip
pip3 install --upgrade pip

# Clone the repository
git clone https://github.com/KianSantang777/KIANPARSER

# Change to project directory
cd KIANPARSER

# Install Python dependencies
pip3 install -r requirements.txt

# Run the tool
python3 dorkparser.py
```
