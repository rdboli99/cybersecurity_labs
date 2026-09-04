# Server Reconnaissance

## Date
### 9/4/2026

## Objective

Identify the operating system, system configuration,
running services, and listening network ports.

## System Information

### Hostname
practiceserver


### Operating System
Ubuntu
Version 26.04 LTS
UBUNTU_CODENAME=resolute

### Kernel
I'm not sure where to find this.

### Current User
rossdboli

### IP Address
10.0.2.15

### RAM
135M available

### Disk


## Running Services

| Service | Status | Purpose |
  ssh.service                 loaded active running OpenBSD Secure Sh>
  - Secure Shell server. Open BSD
  polkit.service              loaded active running Authorization Man>
  - Auth manager
  upower.service              loaded active running Daemon for power >
  - Deamon for power management
  getty@tty1.service          loaded active running Getty on tty1
  - Getty on TTY1. a standard Linux program that manages physical or virtual text terminals, displays the login prompt, and starts the authentication process when a user tries to sign in
  chrony.service              loaded active running chrony, an NTP cl>
  - Chrony is an NTP client/server

## Listening Ports

| Port | Protocol | Service | Expected? |
53 | DNS | Network name resolution | yes |
68 | UDP | default UDP port | yes
22 | SSH | Secure shell | yes
323 | Chrony | Time management | yes

## Initial Assessment
After reconnaissance, I learned that this is an Ubuntu VM server that has SSH active. My initial findings show that this is a training server for junior cybersecurity analysts. 
Further investigation is required to ensure the open ports (DNS, DHCP, SSH) are required and don't pose a threat. 

### Findings
I did not identify any obviously suspicious listening ports during the initial reconnaissance.

### Suspicious Activity
No suspicious activity on this server. 

### Recommended Actions
AT this time, no recommended action is needed other than possible upgrading the RAM space as it seems a bit low. 

## What I Learned
The system is an Ubuntu Server VM configured with SSH access and several system services. Based on the available evidence, no obvious indicators of compromise were identified during initial reconnaissance.

