# CYBER SECURITY INTERNSHIP - TASK 4 REPORT
## Setup and Use a Firewall on Windows/Linux

* **Intern Name:** Mohammed Sufiyan Ahmed
* **Key Concepts:** Firewall Configuration, Network Traffic Filtering, Ports, UFW, Windows Firewall[cite: 14].

---

## 1. Objective
* Configure and test basic firewall rules to allow or block incoming and outgoing network traffic[cite: 14].

## 2. Tools Used
* **Windows Defender Firewall with Advanced Security:** Built-in Windows enterprise-grade traffic filtering tool used for managing inbound and outbound security rules.

## 3. Deliverables
* Screenshots and configuration details showing applied firewall rules (blocking inbound Port 23 / Telnet traffic)[cite: 14].

## 4. Outcome
* Acquired fundamental firewall management skills and a practical understanding of network traffic filtering mechanisms[cite: 14].

---

## 5. Step-by-Step Execution
1. Opened firewall configuration tools using Advanced Security settings (`wf.msc`)[cite: 14].
2. Reviewed existing active inbound and outbound firewall rules[cite: 14].
3. Created a new **Inbound Rule** targeting specific local TCP **Port 23** (Telnet)[cite: 14].
4. Configured the action rule to **Block the connection** across all profiles (Domain, Private, Public)[cite: 14].
5. Named the rule `Block Telnet Port 23` and successfully verified its status in the active rules list[cite: 13, 14].

---

## 6. Interview Questions & Theoretical Answers

1. **What is a firewall?**
   * A network security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules.

2. **Difference between stateful and stateless firewall?**
   * A stateful firewall remembers the context and state of active connections (inspecting packet payloads and connection states), whereas a stateless firewall filters packets independently based solely on static rules (source/destination IPs and ports) without keeping track of connection states.

3. **What are inbound and outbound rules?**
   * Inbound rules control traffic entering your system from an external network, while outbound rules control traffic leaving your system toward an external destination.

4. **How does UFW simplify firewall management?**
   * UFW (Uncomplicated Firewall) provides a user-friendly, command-line frontend interface for managing underlying `iptables` packet filtering rules on Linux systems.

5. **Why block port 23 (Telnet)?**
   * Telnet transmits all data—including usernames and passwords—in cleartext plaintext, making it extremely vulnerable to packet sniffing and credential theft.

6. **What are common firewall mistakes?**
   * Using overly permissive rules (like "Allow All"), failing to log traffic properly, placing rules in the wrong order of evaluation, and neglecting regular rule audits.

7. **How does a firewall improve network security?**
   * By acting as a secure barrier between trusted internal networks and untrusted external networks, blocking unauthorized access attempts and malicious traffic.

8. **What is NAT in firewalls?**
   * Network Address Translation modifies IP address information in packet headers while in transit, allowing multiple devices on a local network to share a single public IP address.

---

## 7. Evidences Collected

### Windows Firewall Rule Configuration Output
```html
<img src="path/to/firewall-rule-block-port-23.png" width="800">
