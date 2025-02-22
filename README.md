# AbdTechO 🛡️

AbdTechO is a cutting-edge cybersecurity tool designed to revolutionize web technology detection and vulnerability assessment. By seamlessly integrating Wappalyzer's robust technology identification with Nuclei's precision security scanning, AbdTechO empowers security professionals to uncover hidden risks and secure their web applications with unparalleled efficiency.

With AbdTechO, you can:

-Automatically Detect Web Technologies: Identify frameworks, CMS platforms, and server technologies in real-time.

-Targeted Vulnerability Scanning: Perform focused security scans based on detected technologies, powered by Nuclei's extensive template library.

-Comprehensive Vulnerability Intelligence: Cross-reference findings with the National Vulnerability Database (NVD) to uncover known CVEs and security flaws.

-Exploit and Threat Enrichment: Gain actionable insights by checking for available exploits in ExploitDB, Vulners, and Metasploit.

-Multi-Domain Scanning: Effortlessly scan multiple domains or subdomains from a single input file.

AbdTechO is more than just a tool—it's your partner in building a secure digital future. Whether you're a penetration tester, security researcher, or IT administrator, AbdTechO equips you with the intelligence and automation needed to stay ahead of evolving threats.


## 📋 Prerequisites

- Python 3.x
- Go (for Nuclei installation)
- Internet connection for NVD API access

## 🔧 Installation

1. Clone the repository:
```bash
git clone https://github.com/abdorhl/AbdTechO.git
cd AbdTechO
````
2. Install Python dependencies:
```bash
pip install -r requirements.txt
```
3. Install Tools
```bash
chmod +x install.sh
./install.sh
```

## 📖 Usage
```bash
usage: AbdTechO.py [-h] [-u URL | -f FILE] [-o OUTPUT]
                   [-s {info,low,medium,high,critical}] [--no-tech] [--ignore-ssl]
                   [-t TECHNOLOGY] [-d]

Detect web technologies and run targeted Nuclei scans

options:
  -h, --help            show this help message and exit
  -u, --url URL         Target URL to scan
  -f, --file FILE       File containing list of subdomains to scan
  -o, --output OUTPUT   Output file to save results (JSON format)
  -s, --severity {info,low,medium,high,critical}
                        Minimum severity level to report
  --no-tech             Skip technology detection and run all Nuclei scans
  --ignore-ssl          Ignore SSL certificate verification
  -t, --technology TECHNOLOGY
                        Specify technology to scan for (e.g., "wordpress", "nginx")
  -d, --debug           Enable debug mode         Skip technology detection and run all Nuclei scan
```

## ⚠️ Disclaimer

This tool is for educational and authorized testing purposes only. Always ensure you have permission to scan the target systems. The authors are not responsible for any misuse or damage caused by this tool.


## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Wappalyzer](https://github.com/AliasIO/Wappalyzer)
- [Nuclei](https://github.com/projectdiscovery/nuclei)
- [NIST NVD](https://nvd.nist.gov/)

---
<p align="center">
Made with ❤️ by PiPaw
</p>
