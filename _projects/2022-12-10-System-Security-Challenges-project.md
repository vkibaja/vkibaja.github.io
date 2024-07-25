---
title: 'System Security Challenges'
subtitle: 'System Security Challenges at Northeastern University'
date: 2022-12-10 00:00:00
description: These are security system challenges I worked on while at Northeastern University.
featured_image: '/images/demo/System-Security.jpg'
---

![](/images/demo/demo-landscape.jpg)

## System Security Challenges

These are **security system challenges** I worked on while at Northeastern University.
* Engaged in weekly practical challenges to develop skills in security assessment, threat modeling, and information protection strategies.
* Created and executed exploits on simulated applications, targeting vulnerabilities like XSS and buffer overflows.
* Gained foundational knowledge in Linux command line, web application security, binary exploitation, reverse engineering, malware analysis, and ethical hacking.

### 1. Buffer Overflow Attack Vulnerability Exploitation

I explored buffer overflow vulnerabilities using a SEED lab environment with Ubuntu 16.04. By disabling critical security features such as address space randomization, stack guard protection, and non-executable stack, I created a controlled setting to exploit a buffer overflow attack. Utilizing gdb for precise memory address identification and constructing a payload with `exploit.c`, I successfully achieved root access.

I also tested and defeated various countermeasures, including address randomization and dash shell's privilege-dropping mechanism, demonstrating a comprehensive understanding of both offensive and defensive aspects of buffer overflow vulnerabilities. For detailed methodologies and results, please refer to the [full documentation](https://vkibaja.github.io/assets/Buffer_Overflow_Attack_VK.pdf) .


### 2. SELinux

I explored the implementation and configuration of SELinux policies to secure a custom binary application named testprog. Initially, the application ran in an unconfined context despite SELinux being in enforcing mode. I investigated this behavior by observing the inherited contexts and created a custom SELinux policy to properly confine the application. The project involved modifying filesystem contexts and policy files to enforce security restrictions effectively.

Through this process, I demonstrated the ability to manage and troubleshoot SELinux contexts and policies, ensuring that the testprog application adhered to the desired security constraints. This hands-on experience highlights my proficiency in enhancing system security using SELinux, providing valuable insights into policy management and enforcement. For a detailed breakdown of each step and the technical intricacies, please refer to the [full documentation](https://vkibaja.github.io/assets/Lab_3_SELinuc_VK.pdf).


### 3. Enhancing Web Application Security Against CSRF Attacks

This challenge focuses on identifying and mitigating Cross-Site Request Forgery (CSRF) vulnerabilities within a web application. By employing a comprehensive approach, the project includes practical demonstrations of CSRF attacks using both GET and POST requests on an Elgg web application hosted via the Apache web server. Key steps involved configuring a virtual environment with Ubuntu, deploying Docker containers, and meticulously monitoring HTTP requests to understand session management and request parameters.

Through detailed analysis and hands-on experiments, various attack scenarios were explored to illustrate how an attacker could manipulate user actions and gain unauthorized control. The challenge also demonstrates countermeasures, including the implementation of SameSite cookie attributes and anti-CSRF tokens, to enhance the security posture of the application. This practical exploration not only showcases the vulnerabilities but also provides robust solutions, making it a valuable resource for improving web application security. Kindly refer to the [full documentation](https://vkibaja.github.io/assets/Web_security_VK.pdf) for more information.


### 4. Android Repackaging Attack 

I explored the concept of Android repackaging attacks by disassembling, modifying, and repackaging an Android APK file to demonstrate how malicious code can be injected. Using a pre-configured Ubuntu environment and a Seed Android VM, I meticulously disassembled the APK file with apktool, injected malicious code into the smali folder, and reassembled the APK. The malicious code was designed to exploit permissions, allowing the modified app to read and write contacts upon triggering a specific event, such as changing the device's time. 

Subsequently, I signed the APK using keytool and jarsigner to ensure it met Android's installation requirements, then installed it on the Android VM to test the attack's effectiveness. The successful execution of the attack resulted in the unauthorized alteration of contacts and demonstrated the potential for tracking the victim's location. This project underscores the importance of stringent application verification processes and highlights vulnerabilities within app distribution platforms like Google Play Store, emphasizing the need for users to download apps only from trusted sources. For comprehensive methodologies and detailed results, please refer to the [complete documentation](https://vkibaja.github.io/assets/Android_Attack_VK.pdf).


### 5. SSH Authentication and Secure File Transfer Project 

In this challenge, our team explored and implemented various SSH (Secure Shell) authentication mechanisms to enhance security in remote server access and file transfers. We began by utilizing traditional password authentication to establish a connection to the master VM, ensuring correct user and group identifiers. Progressing to a more secure method, we generated RSA key pairs and configured public key authentication, allowing passwordless SSH access to the master server. This setup significantly bolstered security by relying on cryptographic keys instead of passwords.

We further demonstrated secure file transfer capabilities using the SCP (Secure Copy) command. By transferring files between local and remote servers, we ensured data integrity and confidentiality through encryption. The project culminated in creating a secure directory on the master server to store transferred files, validated by generating and transferring SHA-256 hash values. This comprehensive approach showcased our ability to implement robust SSH-based security solutions, making it an essential asset for recruiters and hiring managers seeking expertise in cybersecurity and secure network communications. [SSH](https://vkibaja.github.io/assets/TEAM8_SSH-1.pdf).


### 6. Cryptography: Digital Signature Using OpenSSL

In this project, I demonstrated the use of OpenSSL for generating and verifying digital signatures, focusing on enhancing file security and integrity. By creating a digital signature for our Team8_lab2.cast file, I showcased my ability to implement secure hashing and signature verification using the SHA256 algorithm. This involved generating a hash with OpenSSL's `dgst` command and signing it with `rsautl`, ensuring authenticity and integrity.

Additionally, I organized the project efficiently by creating a structured subfolder within our lab environment and generated another signed file using the same private key, further reinforcing my skills in cryptographic practices and systematic project management. This project highlights my technical proficiency in cybersecurity, specifically in the application of digital signatures, and my capability to manage and execute detailed security protocols. For a comprehensive understanding of the methodologies and detailed steps involved, please refer to the complete project documentation. [Cryptography](https://vkibaja.github.io/assets/resubmit.pdf).


### 7. Password Cracking
In the "Password Cracking" challenge, we employed both online and offline techniques to crack various user passwords. Initially, we performed online attacks using a dictionary-based approach, successfully identifying the passwords of Alice and Bob. We then proceeded with offline attacks by obtaining hashed password files from a Docker instance. Using tools like John the Ripper and Hashcat, we executed dictionary and brute-force attacks, uncovering the passwords of several additional users, including complex cases such as Victor and Eugene.

This comprehensive analysis highlights the vulnerabilities inherent in password storage and emphasizes the necessity of robust password policies and protection mechanisms. For further details on the methodologies and results, please refer to the full project documentation. [Password Cracking](https://vkibaja.github.io/assets/lab3_passwd_cracking.pdf).


### 8. Network Basics
In our "Network Basics" project, we successfully configured a Linux VM as a network gateway and DNS server, and implemented robust firewall rules to manage traffic between a NAT and an internal network. Using VirtualBox, we set up two network interfaces for the Linux VM and a single interface for the Windows VM, ensuring seamless communication within the internal network. We configured static IP addresses, enabled IP forwarding, and utilized Bind9 to establish a caching DNS server.

Our firewall setup included detailed iptables rules to route specific types of traffic, such as SSH, DNS, and HTTPS, while blocking other types by default. We conducted extensive testing to verify connectivity and security, ensuring that our configurations allowed internet access and proper routing for established connections. This project showcases our ability to design, configure, and secure a multi-interface network environment, demonstrating practical skills in network management and cybersecurity. [Network Challenge](https://vkibaja.github.io/assets/lab4_network_basics.pdf).


### 9. Buffer Overflow Exploit 2

In this project, I demonstrated the exploitation of buffer overflow vulnerabilities through two practical exercises. In the first exercise, I performed a simple buffer overflow attack on the `login.c` program by overflowing the password buffer with a specific pattern of data to set the `auth_flag` variable to 1, allowing unauthorized access. In the advanced task, I executed a more complex buffer overflow on the `extra.c` program to gain root shell access. This involved crafting a payload with a NOP slide and shellcode, and strategically overwriting the return address to point to the NOP instructions, successfully invoking a root shell.

Through these exercises, I showcased my ability to identify and exploit security vulnerabilities, understand stack memory layout, and employ debugging tools like GDB for address manipulation. This project underscores my technical expertise in cybersecurity and my capability to practically apply theoretical knowledge in real-world scenarios. For a detailed analysis and step-by-step breakdown of these exploits, I invite you to read the full paper. [Buffer Overflow](https://vkibaja.github.io/assets/lab5_bof.pdf).


### 10. Software Security
In our comprehensive software security project, we successfully set up and secured an Apache web server hosted within a Docker container. The process began with generating a self-signed certificate to establish HTTPS communication. We then conducted a thorough vulnerability scan using Nikto, identifying and addressing several critical issues, including unrestricted access to sensitive files, the lack of essential HTTP security headers (such as X-Frame-Options and X-XSS-Protection), and potential exposures through server tokens and ETags.

Our mitigation steps involved configuring server headers to minimize information leakage, securing directories, and updating cipher suites to enhance encryption strength. Additionally, we hardened the operating system by restricting SSH access, enforcing secure password policies, and managing user privileges effectively. This project highlights our ability to identify security weaknesses and implement robust solutions to safeguard web applications against common threats, offering a detailed look into practical security measures in a controlled environment. [Software Security](https://vkibaja.github.io/assets/Lab6_Team8_Software_Security.pdf).


### 11. Database Security 
In my project on database security, I implemented comprehensive measures to secure a MySQL database. I began by creating a new database and securing its data through attribute encryption, ensuring sensitive information like usernames and passwords were protected. I established role-based access control, restricting access based on user roles, and further strengthened security by hardening the database. This included encrypting, hashing, and salting columns in a table to protect critical data such as social security numbers and bank account information. Additionally, I explored automatic encryption mechanisms and leveraged Docker for containerized deployments, enhancing the database's security and ease of management. The project underscores the importance of layered security approaches in safeguarding sensitive data against unauthorized access and breaches. For more details on the methodologies and specific techniques employed, please refer to the full project documentation. [Database Security](https://vkibaja.github.io/assets/Database_Security_VK.pdf).



