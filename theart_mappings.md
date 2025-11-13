---

# 🔐 SentinelNet Threat Detection Mapping

This section outlines how SentinelNet interprets different real-world cyber threats using machine-learning and anomaly-detection signals. It connects **actual attack behavior** to **what our model sees** in network traffic.

---

## 🧩 Threats & Detection Logic

### **1. DDoS Attack**

**What happens:**
Multiple computers flood a server with requests, overwhelming it and causing service disruption.

**How SentinelNet detects it:**

* High traffic volume
* Unusual spikes in connections
* Abnormal flow frequency
* Multiple sources hitting the same target
  ➡️ **Anomaly detection flags this deviation from normal patterns**

---

### **2. Brute-Force Login Attack**

**What happens:**
An attacker repeatedly tries login attempts from the same IP.

**How SentinelNet detects it:**

* Many failed login attempts
* Repeated authentication requests from one source
* Suspicious login behavior sequences
  ➡️ **Classification model identifies repetitive failure signatures**

---

### **3. Port Scanning**

**What happens:**
An attacker scans multiple ports to find open or vulnerable services.

**How SentinelNet detects it:**

* High number of connection attempts on different ports
* Short, incomplete connections
* Sequential or patterned port probing
  ➡️ **Detected as a “suspicious connection pattern”**

---

### **4. Data Exfiltration**

**What happens:**
Sensitive data is transferred out of the network without authorization.

**How SentinelNet detects it:**

* Large outbound data transfers
* Connections to unknown/untrusted external hosts
* Unusual protocols or ports for outbound flows
  ➡️ **Deviation from normal outbound traffic behavior triggers anomaly detection**

---

## ✅ Summary Table

| Real-World Threat     | What Happens                         | How SentinelNet Detects It                                                             |
| --------------------- | ------------------------------------ | -------------------------------------------------------------------------------------- |
| **DDoS Attack**       | Server flooded with traffic          | High traffic spikes & abnormal connection patterns → anomaly detection flags deviation |
| **Brute-Force Login** | Repeated login attempts from same IP | Repeated failed login patterns → model classifies as suspicious                        |
| **Port Scanning**     | Attacker probes many ports           | High number of multi-port attempts → flagged as suspicious pattern                     |
| **Data Exfiltration** | Unauthorized outbound data transfers | Unusual outbound size & destination → detected as abnormal flow                        |

---
