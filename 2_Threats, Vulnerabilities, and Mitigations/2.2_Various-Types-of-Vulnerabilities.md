# 2.2 Explain common threat vectors and attack surfaces

This module focuses on understanding the various pathways or methods (threat vectors) that attackers use to gain unauthorized access to systems or data, and the points or areas (attack surfaces) where an organization is vulnerable to attack. Identifying these helps in designing robust security architectures.

---

## Threat Vectors and Attack Surfaces

### Message-based

Threats delivered through communication channels.

* **Email:**
    * **Description:** The most common vector for delivering malware, phishing links, and social engineering attacks.
    * **Attack Surface:** Email clients, mail servers, user inboxes.
* **Short Message Service (SMS):**
    * **Description:** Used for smishing (SMS phishing) to deliver malicious links or request sensitive information via text messages.
    * **Attack Surface:** Mobile phones, user trust in SMS.
* **Instant messaging (IM):**
    * **Description:** Phishing, malware delivery, or social engineering through platforms like Slack, Microsoft Teams, WhatsApp, etc.
    * **Attack Surface:** IM clients, user accounts, perceived trust within IM platforms.

### Image-based

* **Description:** Malicious code or data hidden within image files (steganography) or images used as part of a malicious campaign (e.g., in a phishing email).
* **Attack Surface:** Image processing software, web browsers displaying images, user interaction with image files.

### File-based

* **Description:** Malware embedded in various file types (e.g., executables, PDFs, Office documents, archives) delivered via email, downloads, or removable media.
* **Attack Surface:** User machines (when files are opened), file servers, file transfer protocols.

### Voice call

* **Description:** Vishing (voice phishing) attempts to trick individuals into revealing sensitive information over the phone.
* **Attack Surface:** Telephony systems, user trust in phone calls.

### Removable device

* **Description:** Malicious software or data spread via USB drives, external hard drives, CDs/DVDs, often when an infected device is plugged into a clean system.
* **Attack Surface:** USB ports, autoplay features, endpoint security.

### Vulnerable software

Software with known or unknown flaws that can be exploited.

* **Client-based vs. agentless:**
    * **Client-based:** Software installed on individual user devices (e.g., web browsers, media players, office suites) that can have vulnerabilities.
    * **Agentless:** Systems that are managed or accessed without installing a dedicated agent on them (e.g., network devices, some cloud services), where vulnerabilities in their native interfaces or protocols can be exploited.
* **Attack Surface:** Any application or service running on a system that processes input or handles data.

### Unsupported systems and applications

* **Description:** Software or hardware that no longer receives security updates or patches from the vendor, making them prime targets for attackers who exploit known, unpatched vulnerabilities.
* **Attack Surface:** End-of-life (EOL) operating systems, legacy applications, outdated hardware.

### Unsecure networks

Networks with weak or improper security configurations.

* **Wireless:**
    * **Description:** Weak encryption (e.g., WEP), misconfigured access points, rogue access points, or unprotected guest networks.
    * **Attack Surface:** Wireless access points, client devices connecting to Wi-Fi.
* **Wired:**
    * **Description:** Lack of network segmentation, insecure switch configurations, ARP poisoning, or unauthorized physical access to network jacks.
    * **Attack Surface:** Network switches, routers, physically accessible ports.
* **Bluetooth:**
    * **Description:** Weak pairing processes, known vulnerabilities in Bluetooth protocols (e.g., Bluejacking, Bluesnarfing), or leaving devices in discoverable mode.
    * **Attack Surface:** Bluetooth-enabled devices (phones, headphones, IoT devices).

### Open service ports

* **Description:** Network ports that are unintentionally left open or misconfigured, allowing direct access to services that should be restricted. These can include unnecessary services running or default ports left open.
* **Attack Surface:** Firewalls, routers, servers, and other network devices with accessible ports.

### Default credentials

* **Description:** Devices or software configured with their original factory usernames and passwords, which are often publicly known or easily guessed.
* **Attack Surface:** Routers, IoT devices, network appliances, web application admin panels.

### Supply chain

Attacks that target an organization through its third-party relationships.

* **Managed service providers (MSPs):**
    * **Description:** Compromising an MSP can provide attackers access to all of the MSP's clients.
    * **Attack Surface:** MSP's infrastructure, shared access to client systems.
* **Vendors:**
    * **Description:** Attacks targeting software vendors to inject malicious code into legitimate software updates (e.g., SolarWinds).
    * **Attack Surface:** Vendor's development environment, software distribution channels.
* **Suppliers:**
    * **Description:** Exploiting vulnerabilities in components, raw materials, or services provided by suppliers.
    * **Attack Surface:** Any third-party component or service integrated into the organization's operations.

### Human vectors/social engineering

Exploiting human psychology to manipulate individuals into performing actions or divulging confidential information.

* **Phishing:**
    * **Description:** Fraudulent attempts to obtain sensitive information by disguising as a trustworthy entity in electronic communication (e.g., email).
* **Vishing:**
    * **Description:** Phishing conducted over voice calls, often using spoofed caller IDs.
* **Smishing:**
    * **Description:** Phishing conducted via SMS text messages.
* **Misinformation/disinformation:**
    * **Misinformation:** Spreading incorrect or misleading information, often unintentionally.
    * **Disinformation:** Deliberate creation and spread of false information to deceive or manipulate.
* **Impersonation:**
    * **Description:** Attacker pretends to be someone else (e.g., a colleague, IT support, a trusted authority) to gain access or information.
* **Business email compromise (BEC):**
    * **Description:** Sophisticated scam targeting businesses working with foreign suppliers or regularly performing wire transfer payments. Attackers compromise legitimate business email accounts to facilitate unauthorized transfers of funds.
* **Pretexting:**
    * **Description:** Creating a believable fabricated scenario (pretext) to trick a target into divulging information or performing an action.
* **Watering hole:**
    * **Description:** Attacker observes which websites a target group frequently visits and infects one of those sites with malware, waiting for the target to visit.
* **Brand impersonation:**
    * **Description:** Attacker mimics a well-known brand (e.g., through fake websites, emails, logos) to trick users into believing they are interacting with the legitimate company.
* **Typosquatting:**
    * **Description:** Registering domain names that are slight variations of legitimate domains, hoping users will type them incorrectly and land on the attacker's malicious site.
