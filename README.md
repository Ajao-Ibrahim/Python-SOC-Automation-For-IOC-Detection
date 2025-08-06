## Python SOC Automation For IOC Detection

##  Objectives
- Automate the detection of Indicators of Compromise (IOCs) in system logs using Python  
- Read and analyze log files exported from Windows and Sysmon  
- Compare logs against known malicious IOCs from threat intelligence   
- Build a simple Python-based SOC automation workflow

---

##  Tools Used

| Tool         | Purpose                                              |
|--------------|------------------------------------------------------|
| Python       | Scripting language for automation                    |
| Pandas       | CSV log reading and data manipulation                |
| Sysmon       | Provides detailed Windows telemetry in logs          |
| Windows 10   | Source of log data for the project                   |
| wireshark    | coverting .pcap file into .csv file                  |


---

##  Steps

1. Set up a working directory for the project  
2. Install Python and required libraries (pandas, re)  
3. Create and populate the iocs.txt file with known IOCs  
4. Export Sysmon logs as logs.csv using Splunk or Event Viewer
5. Use Malware Traffic Analysis to download .pcap file
6. use wireshark for .pcap-to-CSV conversion.
7. Write the main.py script to:
   - Load IOCs  
   - Parse logs  
   - Match IOCs  
   - Output or email alerts  
8. Run the script and analyze output  
---

## Python Script

  <a href="https://github.com/Ajao-Ibrahim/Python-Script/blob/main/README.md?plain=1">main.py</a>

---

##  Sample Detection Use Cases

| Use Case                 | Python Code Snippet                              |
|--------------------------|--------------------------------------------------|
| IP Address Match         | if "192.168.1.6" in str(field):                  |
| Domain Match             | if "malicious.com" in str(field):                |
| Suspicious Process Name  | if "mimikatz.exe" in str(field):                 |
| Encoded PowerShell Usage | if "powershell" in field and "enc" in field:     |

---
## Pictures

---
