# 👃 Packet Sniffer Lab

## Objective

In this project, I built a network packet sniffer to capture and analyze traffic on my local network. The goal was to understand how network packets work, observe live network data, and document the process in a reproducible format suitable for portfolio presentation, while ensuring sensitive information is redacted.

---

### 🧠 Skills Learned

* Used Python and raw sockets to capture live network traffic.
* Analyzed packet headers to extract IP addresses, MAC addresses, ports, and protocol information.
* Interpreted payload data for HTTP, TCP, and UDP traffic.
* Practiced safe data handling by redacting sensitive information in screenshots.
* Documented the lab setup, packet capture, and analysis for reproducibility.

---

### 🛠️ Tools Used

* **Python 3.11+** – primary programming language for the sniffer.
* **Scapy / socket library** – for capturing and analyzing packets.
* **Pandas** - for CSV file loading/manipulation
* **macOS** – host machine for running the sniffer.
* **Canva** – for data sanitizing.

---

## 🧩 Steps

### Step 1: Set Up the Environment

* Installed Python and necessary libraries:

  ```bash
  pip install scapy
  ```
* Prepared a safe testing environment using only dummy traffic where possible.

<img width="633" height="306" alt="scapy" src="https://github.com/user-attachments/assets/c08254f5-57c7-47db-a420-208371061c73" />


---

### Step 2: Capture Network Packets

* Wrote a Python script to capture packets in real time:

<img width="1470" height="956" alt="Screenshot 2025-08-26 at 6 09 31 PM" src="https://github.com/user-attachments/assets/ba5f8d83-e7b0-40c0-b9ed-f64eb3662b89" />

* Observed live traffic including Ethernet, IP, TCP, UDP, and HTTP packets.

<img width="1384" height="414" alt="first results" src="https://github.com/user-attachments/assets/26cd0afb-a7fa-4f5c-aa7a-1b9a5f1760d8" />

---

### Step 3: Filter Packets and Save to CSV

* Wrote a second Python script to filter captured packets by protocol (e.g., TCP, UDP, HTTP) and save relevant data to a CSV file for analysis:

<img width="535" height="499" alt="Screenshot 2025-08-26 at 6 23 37 PM" src="https://github.com/user-attachments/assets/b565db7b-461e-4f19-aa4e-203778c58d54" />


* The CSV captured fields like source and destination IPs, protocol type, and packet length.
* This allowed offline analysis of captured traffic without running the sniffer live.
* Redacted sensitive information in the CSV and screenshots before sharing.

<img width="1474" height="738" alt="second results" src="https://github.com/user-attachments/assets/40ff1b35-a708-4d2c-9feb-df2b51578a03" />

---

If you want, I can **rewrite the full README** now with this updated Step 3 so it accurately reflects both sniffers and the CSV workflow. Do you want me to do that?

### Step 4: Handle Sensitive Data

* Redacted IP addresses, MAC addresses, and any payload containing personal data before sharing.
* Ensured screenshots only show relevant information for demonstration purposes.

---

### Step 5: Document Findings

* Recorded packet types, protocols observed, and notable patterns.
* Included screenshots and redacted captures in README for reproducibility.
* Highlighted practical use cases like monitoring network performance or debugging traffic.

---

### Conclusion

This lab provided hands-on experience in capturing and analyzing network traffic using Python. It reinforced knowledge of networking protocols, packet structures, and safe handling of sensitive information. The project helped me understand packet-level communication, develop skills in network analysis, and document findings in a clear, reproducible format suitable for a portfolio.

