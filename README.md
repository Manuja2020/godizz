# godizz
for url enumeration

# Hacking Tool

A modular Go-based tool for fuzzing, directory enumeration, and vulnerability testing (SQLi, XSS, CSRF, SSRF, LFI).

## Features
- Modular payload support for common vulnerabilities.
- Directory enumeration with custom wordlists.
- High concurrency for quick results.
- Extendable payload sets.

## Usage

```bash
# Install dependencies
go mod tidy

# Run the tool
./hacking-tool --target http://example.com --type sqli --wordlist data/wordlist.txt

# For Linux Based Installations

# Clone the repository
git clone https://github.com/your-username/hacking-tool.git
cd hacking-tool

# Install
chmod +x scripts/install.sh
./scripts/install.sh

# Run the tool
hacking-tool --help

# For Docker Image Based Installation

# Build the Docker image
chmod +x scripts/build-docker.sh
./scripts/build-docker.sh

# Run the tool with Docker
docker run --rm -v $(pwd)/data:/app/data hacking-tool:latest --help

# Example: Run the tool with a target
docker run --rm -v $(pwd)/data:/app/data hacking-tool:latest --target http://example.com --type sqli
