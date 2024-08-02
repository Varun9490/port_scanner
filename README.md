# 🔍 Portscanner

## Description
Portscanner is a simple yet effective Python-based tool designed to scan and identify open ports on a given target. It leverages the `socket` and `termcolor` modules to perform network operations and provide colored terminal outputs, respectively. This tool can scan multiple targets and is particularly useful for network administrators and security professionals for initial reconnaissance and network troubleshooting.

## Installation Instructions
To use Portscanner, you need to have Python installed on your system. Additionally, you'll need to install the required dependencies. Follow the steps below to get started:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/portscanner.git
    cd portscanner
    ```

2. **Install the dependencies:**
    ```bash
    pip install termcolor
    ```

## Usage Guide
To run Portscanner, you need to provide the target(s) you wish to scan and specify the range of ports to be scanned.

1. **Single Target Scan:**
    Simply provide a single IP address or hostname and the number of ports to scan.
    ```bash
    python portscanner.py
    [*] Enter Targets To Scan (split them by ,): 192.168.1.1
    [*] Enter How Many Ports You Want To Scan: 100
    ```

2. **Multiple Targets Scan:**
    Provide multiple IP addresses or hostnames separated by commas and the number of ports to scan.
    ```bash
    python portscanner.py
    [*] Enter Targets To Scan (split them by ,): 192.168.1.1,192.168.1.2
    [*] Enter How Many Ports You Want To Scan: 100
    ```

### Example Command
```bash
python portscanner.py
[*] Enter Targets To Scan (split them by ,): 192.168.1.1, 192.168.1.2
[*] Enter How Many Ports You Want To Scan: 50
```

Output:
```bash
[*] Scanning Multiple Targets
 Starting Scan For 192.168.1.1
[+] Port Opened 22
[+] Port Opened 80
 Starting Scan For 192.168.1.2
[+] Port Opened 22
[+] Port Opened 443
```
