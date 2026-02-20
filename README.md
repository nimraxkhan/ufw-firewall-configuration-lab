🔐 Firewall Configuration Lab – UFW (Kali Linux)
📌 Objective

Configure and validate firewall rules using UFW to control HTTP and HTTPS traffic at the port level.

🛠 Tools Used

Kali Linux

UFW (Uncomplicated Firewall)

curl

Linux Terminal

⚙️ Configuration Steps

Enabled UFW firewall

Verified firewall status

Blocked HTTP traffic (Port 80) – inbound and outbound

Allowed HTTPS traffic (Port 443)

Reloaded firewall rules

Tested enforcement using curl

🔎 Firewall Rules Verification
sudo ufw status verbose

Confirmed:

Port 80 → DENY (IN and OUT)

Port 443 → ALLOW (IN)

🧪 Testing & Validation
❌ HTTP Test (Blocked)
curl http://google.com

Result:
Connection failed → confirms port 80 blocked.

✅ HTTPS Test (Allowed)
curl https://google.com

Result:
HTML returned → confirms port 443 allowed.

📸 Evidence
Firewall Active

Rules Configured

🧠 Skills Demonstrated

Firewall configuration

Port-level access control

Traffic filtering validation

Linux command-line security management

Network security fundamentals

🎯 Key Takeaway

This lab demonstrates practical experience configuring and validating firewall rules to enforce access control policies — a foundational skill in Security Operations and Blue Team environments.
