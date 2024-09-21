- <a href="https://github.com/rafa0c">Home Portfolio</a>

# 🛡️ Scanning with Nmap

## Setup and Prerequisites

1. Install VirtualBox:

Download and install VirtualBox on your machine.
Create virtual machines for both Kali Linux (attacker machine) and Metasploitable 2 (vulnerable target).

2. Set Up Metasploitable2:

Download and install Metasploitable2 from the official repository.
Ensure that both the Kali Linux and Metasploitable 2 VMs are on the same network (NAT or host-only network) so that they can communicate.

3. Set Up Kali Linux:

Download Kali Linux from the official website and install it on VirtualBox.
Update the system by running the following commands:

<pre>   sudo apt update && sudo apt upgrade  </pre>

## Scanning with Nmap
Once your setup is complete, you can use Nmap from the Kali Linux machine to scan the Metasploitable2 machine.

1. **Find the Metasploitable2 IP Address:**

Start Metasploitable2 in VirtualBox.
Run the following command inside the Metasploitable2 virtual mach ine to find the IP address:

<pre>  ifgonfig  </pre>

- Look for the IP under the inet addr section for eth0 (typically something like 192.168.x.x).

2. **Nmap Scan on Kali Linux:**

In Kali Linux, open a terminal and run an Nmap scan targeting Metasploitable 2’s IP address. You can use different scan types depending on what you want to demonstrate.
Here are a few examples:

- 🌐 **Basic scan**(find open ports):

<pre>  nmap [target IP]  </pre>

- 🌐 **Service version detection**:

<pre>  nmap -sV [target IP]  </pre>

- 🌐 **Operating system detection**:

<pre>  nmap -O [target IP]  </pre>

- 🌐 **Aggressive scan** (includes OS detection, version detection, script scanning, and traceroute):

<pre>  nmap -A [target IP] </pre>

3. **Save Results to a File**:

 - 💾 You can save your Nmap scan results to a file using the **_-oN or -oX_** option.
**_Example_**: 

<pre>  nmap -A [target IP] -oN scan_results.txt </pre>

#  Adding Nmap Results
1. **Organize Files**:

Include the Nmap output files (both .txt and .xml if available) in your portfolio.
Add a brief explanation of the results and how they could be useful in vulnerability analysis.

2. **Screenshot Your Process**:

Take screenshots of running the Nmap scan in Kali Linux and discovering open ports and services on Metasploitable 2.
Save these screenshots to include in your portfolio documentation.

3. Write-Up:

Create a document that explains the following:

- The purpose of using Nmap and what you are testing for.
- A summary of the results (e.g., open ports, detected services, and their versions).
- Any interesting findings or vulnerabilities discovered on Metasploitable 2.
- Attach the Nmap output files and screenshots to support your findings.

# 📷  Example Nmap Results 

<pre>  _screenshot of Nmap results_ </pre>

**Conclusion**
After completing the Nmap scan, summarize your findings.
Highlight any vulnerabilities detected, such as open ports or services that are exploitable (e.g., outdated software, insecure services like FTP or Telnet).
Discuss possible attack vectors or defensive strategies to mitigate these risks.





  




  








