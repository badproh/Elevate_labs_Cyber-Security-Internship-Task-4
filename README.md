# Task 4: Firewall Configuration Report

## 1. Objective
To configure and test basic firewall rules to filter network traffic and improve system security by blocking insecure services.

## 2. Configuration Details
* **Platform:** Windows 11
* **Tool Used:** Windows Defender Firewall with Advanced Security
* **Action:** Blocked Inbound Traffic on Port 23 (Telnet)
* **Protocol:** TCP
* **Rule Direction:** Inbound Rule

## 3. Steps Taken
1.  **Open Firewall Tool:** Launched "Windows Defender Firewall with Advanced Security".
2.  **Initiate New Rule:** Navigated to the **Inbound Rules** section and selected "New Rule".
3.  **Select Rule Type:** Chose the **Port** option to filter traffic based on TCP/UDP ports.
4.  **Configure Protocols:** Selected **TCP** and specified specific local port **23** (Telnet).
5.  **Set Action:** Selected **Block the connection** to ensure no traffic can communicate over this insecure port.
6.  **Apply Profiles:** Applied the rule to Domain, Private, and Public network profiles to ensure total coverage.
7.  **Verification:** Verified that the new rule named "Block Telnet Port 23" appeared in the active rules list with a "Block" icon.

## 4. Summary: How Firewalls Filter Traffic
A firewall acts as a security barrier that monitors and controls incoming and outgoing network traffic based on predetermined security rules. It filters traffic through the following process:

1.  **Packet Inspection:** The firewall examines the header of every data packet entering or leaving the network.
2.  **Rule Matching:** It compares the packet's information (Source IP, Destination IP, Port Number, and Protocol like TCP/UDP) against its list of defined rules.
3.  **Action Enforcement:**
    * **Allow:** If the traffic matches an "Allow" rule (e.g., HTTP on port 80), it passes through.
    * **Block/Drop:** If the traffic matches a "Block" rule (like our Telnet port 23 rule) or doesn't match any allowed rule (default deny), the packet is discarded.

By enforcing these rules, the firewall prevents unauthorized access to the system while allowing legitimate communication to continue safely.

## 5. Evidence
<img width="1920" height="1080" alt="Screenshot (533)" src="https://github.com/user-attachments/assets/e9b2411c-a1d8-49f5-9f65-73cab55af2ee" />
<img width="1920" height="1080" alt="Screenshot (535)" src="https://github.com/user-attachments/assets/59b5f841-bafe-4ab8-9272-f07fca0764b6" />
