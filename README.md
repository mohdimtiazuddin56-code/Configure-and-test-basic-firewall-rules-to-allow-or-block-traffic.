# Configure-and-test-basic-firewall-rules-to-allow-or-block-traffic.

Open wf.msc
Inbound Rules

Select Port → Next
TCP → Specific local ports: 23 → Next
Block the connection → Next
Tick all (Domain, Private, Public) → Next
Name: Block Telnet → Finish
<img width="1920" height="1020" alt="Screenshot (30)" src="https://github.com/user-attachments/assets/174ced50-f34b-4676-8d10-e0f24d51c43a" />

# Test the rule
Connection attempt blocked as per firewall rule

# Add rule to alow SSH (port 22) if on Linux.
Not applicable in Windows setup, only for Linux servers

# Remove the test block rule to restore original state
<img width="1920" height="1017" alt="Screenshot (31)" src="https://github.com/user-attachments/assets/7103b826-44f0-47a9-8b5d-3cc7f16a5762" />

Firewall filters network traffic based on rules. Inbound rules block/allow traffic coming in, outbound rules control traffic going out. By blocking Telnet (23), we ensured unauthorized access was denied, while essential services like SSH (22) remain open. This demonstrates how firewalls secure systems by only allowing trusted traffic.
