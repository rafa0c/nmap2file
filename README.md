- <a href="https://github.com/rafa0c">Home Portfolio</a>

# 🛡️ Scanning with Nmap

## Setup and Prerequisites

1. Install VirtualBox:

Download and install VirtualBox on your machine.
Create virtual machines for both Kali Linux (attacker machine) and Metasploitable 2 (vulnerable target).

2. Set Up Metasploitable 2:

Download and install Metasploitable 2 from the official repository.
Ensure that both the Kali Linux and Metasploitable 2 VMs are on the same network (NAT or host-only network) so that they can communicate.

3. Set Up Kali Linux:

Download Kali Linux from the official website and install it on VirtualBox.
Update the system by running the following commands:

<pre>   sudo apt update && sudo apt upgrade  </pre>

## Scanning with Nmap
Once your setup is complete, you can use Nmap from the Kali Linux machine to scan the Metasploitable2 machine.

1. **Find Metasploitable2 IP Address:**

Start Metasploitable2 in VirtualBox.
Run the following command inside Metasploitable2 to find the IP address:

<pre>  ifgonfig  </pre>







