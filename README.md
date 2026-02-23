
# Web Recon Tool

## Overview
The **Web Recon Tool** is a powerful reconnaissance framework designed for penetration testers and security researchers. This tool helps users discover potential vulnerabilities, enumerate subdomains, check HTTP responses, and perform port scanning, all within a single command-line interface.

## Features
- **Port Scanning:** Quickly identify open ports on the target host.
- **Vulnerability Checking:** Perform vulnerability scans on detected open ports using Nmap and Shodan.
- **Subdomain Enumeration:** Discover subdomains associated with the target domain.
- **Directory Discovery:** Find hidden directories on the target web server.
- **HTTP Check:** Validate the HTTP response of the target.

## Getting Started

### Prerequisites
- Go programming language installed (version 1.17 or higher).
- Nmap installed on your system.
- Access to Shodan API (API key required).
- A Linux environment for execution.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/naodEthiop/web_recon_tool.git
   cd web_recon_tool
   ```

2. Set your Shodan API key as an environment variable:
   ```bash
   export SHODAN_API_KEY=your_shodan_api_key
   ```

3. Build the project:
   ```bash
   go build -o web_recon_tool
   ```

### Usage
Run the tool with the following command format:
```bash
./web_recon_tool <command> [options]
```

#### Commands:
- `portscan <host>`: Perform a port scan on the target host.
- `vulncheck <host>`: Check for common vulnerabilities on the target host.
- `subdomain <host>`: Enumerate subdomains of the target host.
- `dir <host>`: Discover directories of the target host.
- `httpcheck <host>`: Check HTTP response.
- `mode`: Run in a recon mode (full or less).

#### Example:
```bash
./web_recon_tool mode --mode full --host example.com
```

## Contributing
Contributions are welcome! If you have suggestions for improvements or new features, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License.

## Author
Coded by: [Naod-Ethiop ](https://github.com/naodEthiop)
Email: fkremariamfentahun66@gmail.com
Telegram: @naod2i



