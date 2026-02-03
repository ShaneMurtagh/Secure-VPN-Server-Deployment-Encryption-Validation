
<h1>Private-Secure-VPN</h1>



<h2>Description</h2>
This project demonstrates how I set up a self-hosted WireGuard Virtual Private Network (VPN) server with a web-based User Interface (UI) for managing VPN clients as an administrator. The VPN was deployed using the WireGuard Easy (wg-easy) GitHub repository on an Ubuntu Linux cloud server hosted as a Virtual Private Server (VPS) through DigitalOcean Droplets. To ensure security and ease of deployment, I used Docker to run wg-easy and bcrypt to hash the web UI login password. WireGuard is an open-source, cross-platform VPN protocol that leverages modern cryptography for secure communication. In addition, I configured a custom domain to point to the VPS, providing convenient and secure access to the wg-easy interface.
<br />

## Objective

The main objective of this project was to deploy a self-hosted WireGuard VPN server on an Ubuntu-based VPS hosted on DigitalOcean. A key goal was to simplify VPN client management by integrating wg-easy, a lightweight web-based interface. The project also aimed to leverage Docker and Docker Compose to containerize the environment, ensuring portability, scalability, and ease of maintenance. Another major objective was to enhance security by implementing bcrypt password hashing for the web UI login, reducing the risk of brute-force and weak password attacks. Additionally, the project involved configuring a custom domain to point to the VPS, providing a user-friendly and secure way to access the management interface. Overall, the project sought to build a secure, private, and cost-effective VPN solution, demonstrating the practicality of self-hosting VPN services for both personal and organizational use.

### Skills Learned


- Gained hands-on experience deploying and managing a self-hosted VPN using WireGuard.
- Strengthened knowledge of Linux server administration on an Ubuntu VPS hosted by DigitalOcean.
- Learned to use Docker and Docker Compose for containerizing and managing applications.
- Configured and managed wg-easy, a web-based interface for simplifying VPN client administration.
- Applied security best practices, including bcrypt password hashing and firewall configuration.
- Practiced DNS and domain management by pointing a custom domain to the VPS.
- Improved understanding of networking and cryptography concepts through WireGuard’s protocol.
- Enhanced overall skills in cloud computing, containerization, and cybersecurity practices.



### Tools Used


- Ubuntu Linux (22.04 LTS) – Operating system for the VPS server environment.
- DigitalOcean Droplet – Cloud-based Virtual Private Server (VPS) hosting provider.
- WireGuard – Open-source VPN protocol providing secure and fast connectivity.
- wg-easy – Web-based management interface for WireGuard VPN clients.
- Docker – Containerization platform used to run wg-easy efficiently.
- Docker Compose – Tool for defining and managing multi-container Docker applications.
- bcrypt – Password hashing algorithm used to secure the wg-easy web UI.
- Domain Name System (DNS) – Configured to point a custom domain to the VPS for web access.
- UFW (Uncomplicated Firewall) – Used to configure firewall rules and allow VPN/UI traffic.
- PuTTY – Secure Shell (SSH) client used to connect to and manage the VPS remotely.
- <b>https://github.com/wg-easy/wg-easy?tab=readme-ov-file</b>

<h2> The Steps:</h2>

<p align="center">
Virtual private server : <br/>
<img src="https://i.imgur.com/Mo5nLOR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 
 <b>To start I used a vps provider (Oceandrop) to purchace some cloud computing. I chose a basic plan with regular ssd and 1000gb memory priced at 6$ a month. I set the server location to New York city. I selected the latests version of ubuntu for the vps. And chose password as Authentication method and set the password for the vps

