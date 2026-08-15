# Ubuntu Server Lab — Evidence

This folder contains screenshots documenting system enumeration, network configuration and firewall verification performed during the Ubuntu Server lab

## Evidence

### 01 — Hostname Verification

**File:** `system-enumeration-hostname.png`

Shows the Ubuntu Server hostname being identified using the Linux command line. This confirms the server's system identity within the lab environment

### 02 — IP Address Verification

**File:** `system-enumeration-ip-addr.png`

Shows the server's network interfaces and assigned IP addresses using `ip addr`. This was used to verify the server's network configuration

### 03 — Routing Table Verification

**File:** `system-enumeration-ip-route.png`

Shows the server's routing table using `ip route`. This was used to verify the default gateway and available network routes

### 04 — Listening Services Enumeration

**File:** `listening-services-ss-tuln.png`

Shows listening network services and ports using `ss -tuln`. This was used to identify services listening for network connections on the Ubuntu Server

### 05 — UFW Firewall Status

**File:** `firewall-ufw-status.png`

Shows the status of the Ubuntu Uncomplicated Firewall (UFW), including whether the firewall is active and its current configuration

### 06 — Firewall Final Verification

**File:** `firewall-final-verification.png`

Shows the final firewall verification performed after configuring the Ubuntu Server firewall. This provides evidence that the firewall configuration was checked and functioning as intended

## Purpose

The evidence demonstrates practical Linux system administration, network enumeration, routing verification, service enumeration, and host-based firewall management performed during the lab
