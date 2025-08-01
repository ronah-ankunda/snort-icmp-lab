## Snort 3 lab demo for ICMP alerting and rule validation 
# Snort ICMP Alert Lab
This mini project demonstrates how to detect ICMP traffic using Snort 3 on Kali Linux in a virtualized lab environment. It simulates an intrusion detection scenario, showcasing custom rule creation, configuration testing, and output analysis.

## 🧪 Lab Environment
- **Operating System**: Kali Linux 
- **Tool**: Snort (installed manually via terminal)
- **Scenario**: ICMP rule validation and configuration testing using Snort’s test mode (`-T`). No live network traffic was generated. The focus was on ensuring the detection engine correctly interprets and loads a custom ICMP alert rule for SOC-style readiness.
## Custom Snort Rule Used
alert icmp any any -> any any (msg:"ICMP Packet Detected"; sid:1000001; rev:1;)

## Steps Perfomed
1. Installed Snort 3 manually via apt
2. Created a custom rule in `local.rules` to trigger on any ICMP traffic
3. Verified rule integrity using Snort’s test mode
4. Observed alerts via Snort’s console in real-time
5. Captured outputs and screenshots for evidence

## Rule Validation
- Used interface: `eth0`
- Rule file: `/etc/snort/rules/local.rules`
- Loaded: 298 rules (no errors)
- Alert: Successfully triggered and logged to console

## Demo evidence 
This project includes a video demonstration showing:

- Snort rule creation and configuration
- Real-time alert triggering in Snort console
- Validation steps using Snort’s test mode

🎥 [Snort ICMP Alert Lab Demo](https://youtu.be/dRXjBWnZUHA)

> The video walks through the full lab setup and confirms successful detection of ICMP packets using a custom Snort rule.

## 📘 Learning Outcomes
- Gained hands-on experience with Snort rule syntax
- Practiced configuration testing and rule validation using test mode
- Understood how Snort handles rule parsing and readiness checks
- Built foundational skills relevant to SOC alerting and IDS analysis
