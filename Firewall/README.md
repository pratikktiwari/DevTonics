# 🧱🔥 Firewall Cheatsheet
A firewall is a network security device that monitors and controls incoming and outgoing traffic based on predetermined security rules, acting as a barrier between trusted internal networks and untrusted external networks.

It helps prevent unauthorized access, data breaches, and cyber attacks by filtering traffic and blocking harmful activities. Firewalls are essential for maintaining network security and protecting sensitive information.


👉 [Check out the LinkedIn Post](https://www.linkedin.com/posts/devtonics_cybersecurity-networksecurity-firewall-activity-7215041018042155008-03yl)

👉 [Instagram Slide](https://www.instagram.com/p/C9EWgeYSpM3/)

👉 [Follow on LinkedIn](https://linkedin.com/company/DevTonics)

👉 [Career in CyberSecurity](https://devtonics.in/en/security/unveiling-the-world-of-cybersecurity-a-rewarding-career-path-with-options-for-everyone)

### Key Functions of a Firewall

1.  **Traffic Filtering:**
    
    -   Firewalls filter network traffic by allowing or blocking data packets based on a set of security rules. These rules are typically defined by network administrators.
2.  **Access Control:**
    
    -   Firewalls enforce access control policies by permitting or denying traffic to and from specific IP addresses, port numbers, and protocols.
3.  **Monitoring and Logging:**
    
    -   Firewalls monitor network traffic and log relevant data for analysis. This helps in identifying and troubleshooting security incidents and network issues.
4.  **Protection from External Threats:**
    
    -   Firewalls protect internal networks from external threats such as hackers, viruses, and malware by blocking unauthorized access attempts.

### 🔥Types of Firewalls

1.  **Packet-Filtering Firewalls:**
    
    -   Inspect packets at the network layer and filter them based on source and destination IP addresses, port numbers, and protocols.
    -   Simple and efficient but may not detect more complex attacks.
2.  **Stateful Inspection Firewalls:**
    
    -   Track the state of active connections and make filtering decisions based on the context of the traffic.
    -   More secure than packet-filtering firewalls as they consider the state of the connection.
3.  **Proxy Firewalls:**
    
    -   Act as intermediaries between users and the services they access, examining all traffic and filtering it before allowing it to pass through.
    -   Provide a higher level of security by hiding the internal network from external networks.
4.  **Next-Generation Firewalls (NGFWs):**
    
    -   Combine traditional firewall functions with additional features such as deep packet inspection, intrusion prevention, and application-level inspection.
    -   Offer advanced threat detection and prevention capabilities.

### Benefits of Using a Firewall

-   **Enhanced Security:** Firewalls provide a strong defense against unauthorized access and cyber threats.
-   **Traffic Management:** They help in managing and controlling network traffic, ensuring that only legitimate traffic is allowed.
-   **Policy Enforcement:** Firewalls enforce organizational security policies, ensuring compliance with regulatory requirements.
-   **Monitoring and Alerting:** Firewalls offer monitoring and alerting capabilities, providing visibility into network activity and potential threats.

### How Firewalls Work

1.  **Rule-Based Filtering:**
    
    -   Firewalls use a set of predefined rules to allow or block traffic. These rules are based on criteria such as IP addresses, port numbers, and protocols.
2.  **Stateful Inspection:**
    
    -   Stateful firewalls maintain a state table that tracks active connections. They make decisions based on the state of the connection, providing a higher level of security.
3.  **Deep Packet Inspection (DPI):**
    
    -   Next-generation firewalls use DPI to inspect the content of data packets, allowing them to detect and block malicious traffic more effectively.
4.  **Network Address Translation (NAT):**
    
    -   Firewalls often perform NAT, which translates private IP addresses to a public IP address. This helps in hiding the internal network structure from external entities.

By implementing firewalls, organizations can protect their networks from a wide range of threats, ensuring the integrity, confidentiality, and availability of their data and systems.

Security rules in a firewall, also known as firewall rules or access control lists (ACLs), define the criteria for allowing or blocking network traffic. These rules are crucial for maintaining network security and controlling access to resources. Here's a breakdown of what these rules typically involve:

### Components of Firewall Security Rules

1.  **Source IP Address:**
    
    -   Specifies the IP address or range of addresses from which the traffic originates.
2.  **Destination IP Address:**
    
    -   Specifies the IP address or range of addresses to which the traffic is directed.
3.  **Source Port:**
    
    -   Indicates the port number or range of ports on the source device from which the traffic originates.
4.  **Destination Port:**
    
    -   Indicates the port number or range of ports on the destination device to which the traffic is directed.
5.  **Protocol:**
    
    -   Defines the type of protocol being used (e.g., TCP, UDP, ICMP).
6.  **Action:**
    
    -   Specifies the action to be taken when the traffic matches the rule criteria. Common actions include:
        -   **Allow:** Permits the traffic to pass through the firewall.
        -   **Deny:** Blocks the traffic from passing through the firewall.
        -   **Log:** Records the traffic event for monitoring and analysis.

### Types of Security Rules

1.  **Inbound Rules:**
    
    -   Control traffic coming into the network from external sources. These rules are crucial for protecting the network from external threats.
2.  **Outbound Rules:**
    
    -   Control traffic leaving the network. These rules help manage and secure outgoing traffic and can prevent internal systems from communicating with known malicious destinations.
3.  **Default Rules:**
    
    -   Often set to block all traffic unless explicitly allowed. These rules act as a catch-all to ensure any traffic not matching specific rules is denied.

### Examples of Firewall Security Rules

1.  **Allow HTTP Traffic:**
    
    -   **Source IP:** Any
    -   **Destination IP:** Internal Web Server IP
    -   **Source Port:** Any
    -   **Destination Port:** 80 (HTTP)
    -   **Protocol:** TCP
    -   **Action:** Allow
2.  **Deny External FTP Access:**
    
    -   **Source IP:** Any
    -   **Destination IP:** Any
    -   **Source Port:** Any
    -   **Destination Port:** 21 (FTP)
    -   **Protocol:** TCP
    -   **Action:** Deny
3.  **Allow SSH from Specific IP:**
    
    -   **Source IP:** Admin's IP Address
    -   **Destination IP:** Server IP
    -   **Source Port:** Any
    -   **Destination Port:** 22 (SSH)
    -   **Protocol:** TCP
    -   **Action:** Allow
4.  **Block P2P Traffic:**
    
    -   **Source IP:** Any
    -   **Destination IP:** Any
    -   **Source Port:** Any
    -   **Destination Port:** P2P Ports
    -   **Protocol:** Any
    -   **Action:** Deny

### Best Practices for Creating Security Rules

1.  **Principle of Least Privilege:**
    
    -   Only allow access that is necessary for legitimate purposes. Deny all other traffic by default.
2.  **Regular Review and Update:**
    
    -   Periodically review and update firewall rules to ensure they remain effective and relevant.
3.  **Logging and Monitoring:**
    
    -   Enable logging for critical rules to monitor and analyze traffic patterns and potential security incidents.
4.  **Segmentation:**
    
    -   Use different sets of rules for different network segments to provide layered security and minimize the impact of a breach.
5.  **Documentation:**
    
    -   Maintain clear and detailed documentation of all firewall rules, including the rationale behind each rule and the impact on network traffic.

By carefully defining and managing firewall security rules, organizations can effectively control network access, protect against unauthorized access, and mitigate various security threats.

> **Not using a firewall exposes an organization to several significant risks, two of the top risks include:**

### 1. Unauthorized Access and Data Breaches

**Description:** Without a firewall, there is no barrier between your internal network and the outside world. This lack of protection makes it easy for cybercriminals to gain unauthorized access to your systems and data.

**Consequences:**

-   **Data Theft:** Sensitive information such as customer data, financial records, and intellectual property can be stolen.
-   **Loss of Privacy:** Confidential data can be exposed, leading to privacy violations and potential legal ramifications.
-   **Reputational Damage:** A data breach can severely damage an organization’s reputation, resulting in loss of customer trust and potential revenue loss.
-   **Financial Loss:** The cost of mitigating a data breach, including legal fees, fines, and recovery costs, can be substantial.

### 2. Exposure to Malware and Cyber Attacks

**Description:** Without a firewall, your network is more vulnerable to various forms of malware, including viruses, worms, and ransomware, as well as direct cyber attacks such as Distributed Denial of Service (DDoS) attacks.

**Consequences:**

-   **Malware Infections:** Malware can spread across your network, corrupting or destroying data, disrupting operations, and causing significant downtime.
-   **Ransomware Attacks:** Attackers can encrypt your data and demand a ransom for its release, which can halt business operations and incur significant costs.
-   **DDoS Attacks:** Cybercriminals can overwhelm your network with traffic, rendering your services unavailable and disrupting business continuity.
-   **System Compromise:** Attackers can exploit vulnerabilities in your systems, leading to further security breaches and potential control over your network.

### Mitigation Strategies

To mitigate these risks, it is essential to implement a robust firewall solution as part of your overall cybersecurity strategy. This should include:

-   **Regular Updates:** Ensure that firewall software and hardware are regularly updated to protect against the latest threats.
-   **Proper Configuration:** Configure firewall rules to allow only necessary traffic and block potential threats.
-   **Monitoring and Alerts:** Continuously monitor firewall logs and set up alerts for suspicious activities to respond quickly to potential threats.
-   **Layered Security:** Combine firewalls with other security measures such as Intrusion Detection Systems (IDS), Intrusion Prevention Systems (IPS), and antivirus software for comprehensive protection.

## Firewall Rules & Commands

### `iptables` Policies

**1. Basic Commands**
<pre><code># Check current rules
sudo iptables -L

# Flush all rules
sudo iptables -F</code></pre> 

**2. Default Policies**
<pre><code># Set default policy to DROP for input, forward, and output
sudo iptables -P INPUT DROP
sudo iptables -P FORWARD DROP
sudo iptables -P OUTPUT DROP

# Set default policy to ACCEPT for input, forward, and output
sudo iptables -P INPUT ACCEPT
sudo iptables -P FORWARD ACCEPT
sudo iptables -P OUTPUT ACCEPT</code></pre> 

**3. Allow/Deny Specific IP**
<pre><code># Allow traffic from a specific IP
sudo iptables -A INPUT -s 192.168.1.100 -j ACCEPT

# Deny traffic from a specific IP
sudo iptables -A INPUT -s 192.168.1.100 -j DROP</code></pre> 

**4. Allow/Deny Specific Port**
<pre><code># Allow traffic on port 22 (SSH)
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT

# Deny traffic on port 22 (SSH)
sudo iptables -A INPUT -p tcp --dport 22 -j DROP</code></pre> 

**5. Allow/Deny Specific Protocol**
<pre><code># Allow ICMP (ping) traffic
sudo iptables -A INPUT -p icmp -j ACCEPT

# Deny ICMP (ping) traffic
sudo iptables -A INPUT -p icmp -j DROP</code></pre> 

**6. Save and Restore Rules**
<pre><code># Save iptables rules
sudo iptables-save > /etc/iptables/rules.v4

# Restore iptables rules
sudo iptables-restore < /etc/iptables/rules.v4</code></pre> 

### `ufw` Policies

**1. Basic Commands**
<pre><code># Enable ufw
sudo ufw enable

# Disable ufw
sudo ufw disable

# Check status
sudo ufw status</code></pre> 

**2. Default Policies**
<pre><code># Set default policy to deny incoming traffic
sudo ufw default deny incoming

# Set default policy to allow outgoing traffic
sudo ufw default allow outgoing</code></pre> 

**3. Allow/Deny Specific IP**
<pre><code># Allow traffic from a specific IP
sudo ufw allow from 192.168.1.100

# Deny traffic from a specific IP
sudo ufw deny from 192.168.1.100</code></pre> 

**4. Allow/Deny Specific Port**
<pre><code># Allow traffic on port 22 (SSH)
sudo ufw allow 22/tcp

# Deny traffic on port 22 (SSH)
sudo ufw deny 22/tcp</code></pre>

**5. Allow/Deny Specific Service**
<pre><code># Allow HTTP traffic
sudo ufw allow http

# Deny HTTP traffic
sudo ufw deny http

# Allow HTTPS traffic
sudo ufw allow https

# Deny HTTPS traffic
sudo ufw deny https</code></pre>

**6. Allow/Deny Specific IP Range**

<pre><code> # Allow traffic from a specific IP range
sudo ufw allow from 192.168.1.0/24

# Deny traffic from a specific IP range
sudo ufw deny from 192.168.1.0/24</code></pre>

**7. Reset ufw Rules**

<pre><code># Reset all ufw rules to default
sudo ufw reset</code></pre>

### Example `iptables` Configuration

_Allow SSH, HTTP, and HTTPS Traffic_

<pre><code>sudo iptables -P INPUT DROP
sudo iptables -P FORWARD DROP
sudo iptables -P OUTPUT ACCEPT

sudo iptables -A INPUT -m conntrack --ctstate ESTABLISHED,RELATED -j ACCEPT
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT
sudo iptables -A INPUT -p tcp --dport 80 -j ACCEPT
sudo iptables -A INPUT -p tcp --dport 443 -j ACCEPT

sudo iptables -A INPUT -i lo -j ACCEPT</code></pre>

**Save above configuration:**

`sudo iptables-save > /etc/iptables/rules.v4` 

### Example `ufw` Configuration:

_Allow SSH, HTTP, and HTTPS Traffic_

<pre><code>sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw allow 22/tcp
sudo ufw allow 80/tcp
sudo ufw allow 443/tcp
sudo ufw enable</code></pre>

## Some lesser-known but important commands and concepts for managing firewalls in Linux using `iptables` and `ufw`.


### `iptables` Advanced Commands

**1. Rate Limiting:** Prevents certain types of DoS attacks by limiting the number of connections.

<pre><code># Limit SSH connections to 3 per minute per IP

sudo iptables -A INPUT -p tcp --dport 22 -m conntrack --ctstate NEW -m recent --set

sudo iptables -A INPUT -p tcp --dport 22 -m conntrack --ctstate NEW -m recent --update --seconds 60 --hitcount 4 -j DROP</code></pre>

**2. Logging Dropped Packets:** Logs packets that are dropped by the firewall rules for auditing and debugging.

<pre><code>sudo iptables -A INPUT -m limit --limit 5/min -j LOG --log-prefix "iptables denied: " --log-level 7

sudo iptables -A INPUT -j DROP</code></pre>

**3. NAT and Port Forwarding:** Forwards traffic from one port to another port.

<pre><code># Forward port 80 to port 8080 on the same machine

sudo iptables -t nat -A PREROUTING -p tcp --dport 80 -j REDIRECT --to-port 8080

# Forward traffic from port 80 on public IP to port 80 on internal IP

sudo iptables -t nat -A PREROUTING -d <public_ip> -p tcp --dport 80 -j DNAT --to-destination <internal_ip>:80

sudo iptables -A FORWARD -p tcp -d <internal_ip> --dport 80 -j ACCEPT</code></pre>

**4. IP Address Spoofing Protection:** 
Prevents IP address spoofing by dropping packets that claim to be from your internal network but arrive from an external interface.

<pre><code>sudo iptables -A INPUT -i eth0 -s 192.168.1.0/24 -j DROP</code></pre>

**5. Preventing Syn Flood Attacks:** Mitigates SYN flood attacks by limiting the number of SYN packets.

<pre><code>sudo iptables -A INPUT -p tcp --syn -m limit --limit 1/s --limit-burst 3 -j ACCEPT

sudo iptables -A INPUT -p tcp --syn -j DROP</code></pre>

**6. Save and Restore Commands:**

<pre><code># Save rules for IPv6
sudo ip6tables-save > /etc/iptables/rules.v6

# Restore rules for IPv6
sudo ip6tables-restore < /etc/iptables/rules.v6</code></pre>

### `ufw` Advanced Commands

**1. Application Profiles:**  `ufw` uses predefined profiles for common applications, simplifying rule creation.

<pre><code># List available application profiles
sudo ufw app list

# Allow traffic for an application profile
sudo ufw allow 'OpenSSH'</code></pre>

**2. Advanced Rule Syntax:** Create more granular rules specifying interfaces and multiple ports.

<pre><code># Allow HTTP traffic on a specific interface
sudo ufw allow in on eth0 to any port 80

# Allow multiple ports
sudo ufw allow 3000:4000/tcp</code></pre>

**3. Rate Limiting:** Limits the number of connections per IP to prevent brute force attacks.
<pre><code>sudo ufw limit ssh/tcp</code></pre>

**4. Logging:** Enables logging to monitor and audit traffic.

<pre><code># Enable logging (low, medium, high, full)
sudo ufw logging on

# Set logging level
sudo ufw logging medium</code></pre>

**5. Deny Incoming Traffic to Specific IP:**
<pre><code>sudo ufw deny from 203.0.113.0/24</code></pre>

**6. IPv6 Support:** Ensure that `ufw` is configured to handle IPv6 traffic.

<pre><code># Edit the ufw configuration file
sudo nano /etc/default/ufw
# Set IPV6=yes</code></pre>

**7. Resetting `ufw` while Keeping Rules:** Resets `ufw` to default while keeping existing rules.

<pre><code>sudo ufw --force reset</code></pre>

**8. Allow Traffic from Specific Subnet:**

<pre><code>sudo ufw allow from 192.168.1.0/24</code></pre>

### General Best Practices

**1. Backup Configuration:** Always backup your firewall configuration before making changes.

<pre><code># iptables
sudo iptables-save > /path/to/backup/iptables.backup
# ufw
sudo cp /etc/ufw/user.rules /path/to/backup/user.rules.backup</code></pre>

**2. Testing New Rules:** Test new rules on a non-production environment before applying them to live systems to avoid accidental lockouts.

**3. Documentation:** Document all firewall rules and configurations for auditing and troubleshooting purposes.

**4. Regular Audits:** Regularly audit and update firewall rules to ensure they meet current security requirements and reflect changes in your network infrastructure.

By using these advanced commands and best practices, you can enhance the security and functionality of your Linux firewall configuration.
