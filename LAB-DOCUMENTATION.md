# Ubuntu Server – Linux Administration & Networking Lab

## 1. Lab Overview

This project involved configuring and administering an Ubuntu Server in a virtualised lab environment

The lab focused on practical Linux system administration, network configuration and verification, service enumeration, and host-based firewall management

The purpose was to develop hands-on experience using the Linux command line to inspect and manage a server's system and network configuration

---

## 2. Objectives

The main objectives of the lab were to:

* Identify and verify the Ubuntu Server hostname
* Inspect network interfaces and IP addressing
* Verify the server's routing configuration
* Identify listening network services and ports
* Check and manage the UFW firewall
* Perform final firewall verification
* Use Linux command-line tools for system and network administration
* Document the configuration and verification process

---

## 3. Environment and Tools

### Operating System

* Ubuntu Server

### Virtualisation

* VirtualBox

### Tools and Utilities

* Linux Terminal
* Netplan
* UFW (Uncomplicated Firewall)
* `ip`
* `ss`

---

## 4. System Enumeration

System enumeration was performed to understand the server's identity and network configuration before reviewing its exposed services and firewall status

### Hostname

The server hostname was checked using:

```text
hostname
```

This confirmed the identity of the Ubuntu Server within the lab environment

**Evidence:** `01-system-enumeration-hostname.png`

---

## 5. Network Interface and IP Address Verification

The server's network interfaces and assigned IP addresses were inspected using:

```text
ip addr
```

This command was used to identify the available network interfaces and verify their assigned addresses

Understanding the interface and IP configuration is important when troubleshooting connectivity and confirming that the server is connected to the intended network

**Evidence:** `02-system-enumeration-ip-addr.png`

---

## 6. Routing Configuration

The routing table was checked using:

```text
ip route
```

This provided information about the server's network routes and default gateway

Verifying the routing table is an important troubleshooting step because incorrect or missing routes can prevent a server from communicating with other networks

**Evidence:** `03-system-enumeration-ip-route.png`

---

## 7. Listening Services and Ports

Listening network services were enumerated using:

```text
ss -tuln
```

The command was used to identify ports on which services were listening for network connections

This is useful from both an administration and security perspective because it helps identify which network services are exposed on the server

**Evidence:** `04-listening-services-ss-tuln.png`

---

## 8. UFW Firewall

The Ubuntu Uncomplicated Firewall (UFW) was used to manage and verify the host firewall configuration

The firewall status was checked using:

```text
sudo ufw status
```

This allowed the current firewall state and configured rules to be reviewed

**Evidence:** `05-firewall-ufw-status.png`

---

## 9. Final Firewall Verification

A final verification was performed after the firewall configuration to confirm the resulting firewall state

This provided a final check that the intended firewall configuration was active and that the server's host-based firewall was functioning as expected

**Evidence:** `06-firewall-final-verification.png`

---

## 10. Administration and Verification Workflow

The general workflow followed during the lab was:

1. Identify the Ubuntu Server hostname
2. Inspect network interfaces and IP addresses
3. Verify the routing table and default gateway
4. Enumerate listening network services
5. Check the UFW firewall status
6. Review the firewall configuration
7. Perform final firewall verification
8. Capture screenshots as evidence
9. Document the configuration and results

---

## 11. Commands Used

### Hostname

```text
hostname
```

**Purpose:** Identifies the hostname of the Ubuntu Server

### IP Address and Interface Information

```text
ip addr
```

**Purpose:** Displays network interfaces and assigned IP addresses

### Routing Table

```text
ip route
```

**Purpose:** Displays the server's routing table and default route

### Listening Services

```text
ss -tuln
```

**Purpose:** Displays listening TCP and UDP ports

### Firewall Status

```text
sudo ufw status
```

**Purpose:** Displays the current UFW firewall status and rules

---

## 12. Skills Demonstrated

This lab provided practical experience with:

* Linux Server Administration
* Ubuntu Server
* Linux Command Line
* Network Interface Configuration
* IP Addressing
* Routing
* Network Service Enumeration
* Port Enumeration
* Host-Based Firewall Management
* UFW
* Network Troubleshooting
* Security Awareness
* Technical Documentation

---

## 13. What I Learned

This lab strengthened my understanding of Linux server administration and the importance of verifying a system from multiple perspectives

I learned how to inspect a server's identity, network interfaces, IP addressing, routing configuration, and listening services using standard Linux command-line tools

I also gained practical experience with UFW and learned the importance of checking firewall status and performing a final verification after configuration

The lab reinforced a systematic troubleshooting approach:

Identify - Inspect - Verify - Configure - Test

This approach helps avoid making assumptions about a server's configuration and provides a structured way to investigate networking and security issues

---

## 14. Evidence

Screenshots documenting the lab are stored in the:

**`evidence/`**

folder

The evidence includes:

1. Hostname verification
2. IP address and interface verification
3. Routing table verification
4. Listening service enumeration
5. UFW firewall status
6. Final firewall verification

The `README-EVIDENCE.md` file provides captions explaining what each screenshot demonstrates

---

## 15. Key Takeaway

This project provided hands-on experience administering an Ubuntu Server and using Linux command-line tools to inspect networking, routing, listening services, and firewall configuration

The lab also demonstrated the importance of verification and systematic troubleshooting when managing a server environment
