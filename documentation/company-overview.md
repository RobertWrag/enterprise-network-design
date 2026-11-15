# Company Overview

## 1. Company Profile

**Company Name:** Adriatic Tech Solutions d.o.o.  
**Industry:** Software Development, IT Consulting, and Business Analytics  
**Headquarters:** Zagreb, Croatia  
**Branch Office:** Split, Croatia  
**Total Employees:** 250

Adriatic Tech Solutions d.o.o. is a fictional technology company specializing in software development, IT consulting, and business analytics. The company operates from two locations in Croatia: its headquarters in Zagreb and a regional branch office in Split.

The company relies on a stable, secure, and scalable IT infrastructure to support internal business operations, software development activities, customer support, and communication between its offices.

This project focuses on designing an enterprise network infrastructure that connects both locations and provides secure access to internal resources for employees working on-site and remotely.

## 2. Company Locations

### 2.1 Zagreb – Headquarters

The Zagreb headquarters employs approximately 200 people and hosts the company's main office, central IT administration, and primary data center.

The headquarters provides centralized infrastructure and services for both company locations.

**Department distribution:**

| Department | Employees |
|---|---:|
| Research & Development (R&D) | 90 |
| Customer Support & Operations | 45 |
| Sales & Marketing | 30 |
| Finance, Legal & HR | 20 |
| IT Administration & Security | 10 |
| Management | 5 |
| **Total** | **200** |

**Main responsibilities:**
- Central IT infrastructure management.
- Software development and testing.
- Customer support and business operations.
- Centralized data and application hosting.
- Network and security administration.

### 2.2 Split – Branch Office

The Split branch employs approximately 50 people and focuses on regional sales, customer support, and administrative activities.

The branch connects to the Zagreb headquarters through a dedicated site-to-site VPN connection.

**Department distribution:**

| Department | Employees |
|---|---:|
| Regional Sales & Marketing | 20 |
| Technical Support – Tier 1 | 20 |
| Administration & Local IT | 10 |
| **Total** | **50** |

**Main responsibilities:**
- Regional sales and customer relations.
- First-level technical support.
- Local administrative operations.
- Basic local IT support.

The Split office uses centralized services hosted in Zagreb while maintaining selected local infrastructure services to support branch operations.

## 3. IT Infrastructure Overview

The company operates a hybrid IT environment consisting of centralized infrastructure, local network resources, and remote access capabilities.

### 3.1 Central Data Center – Zagreb

The primary data center is located at the Zagreb headquarters.

It hosts essential internal services, including:

| Service | Purpose |
|---|---|
| Active Directory (AD) | Centralized user and computer authentication |
| DNS | Internal name resolution |
| DHCP | Dynamic IP address allocation |
| Git Server | Source code management and collaboration |
| Database Servers | Storage and management of business application data |
| Application Servers | Hosting internal business applications |

These services are primarily accessible through the corporate network and authorized connections from the Split branch.

### 3.2 Local Infrastructure – Split

The Split branch maintains a limited set of local services to support daily operations.

Planned local services include:
- Read-Only Domain Controller (RODC).
- Local file and print services.
- Network printers and access control devices.

Centralized authentication and access to corporate resources remain managed through the Zagreb headquarters.

### 3.3 Public-Facing Infrastructure

The company requires selected services to be accessible from external networks.

These services are planned to operate within a dedicated Demilitarized Zone (DMZ).

Planned components include:
- Public-facing web services.
- VPN connectivity infrastructure.
- Mail gateway.
- Reverse proxy.

Public-facing services must be isolated from internal corporate and server networks through appropriate network security controls.

## 4. Workforce and Connectivity Requirements

The company supports both traditional office-based work and hybrid working arrangements.

Employees require reliable access to:
- Internal business applications.
- Shared files and databases.
- Development and collaboration platforms.
- Email and communication services.
- Internet resources.
- Voice communication systems.

Remote employees must be able to securely access authorized internal resources through Remote Access VPN.

Access permissions should depend on the employee's role and business requirements.

## 5. Network Infrastructure Requirements

The enterprise network must support the following infrastructure components:

### 5.1 Corporate LAN

The corporate LAN provides connectivity for employee workstations and business devices.

Departments must be logically separated using VLANs to improve security, manageability, and traffic control.

### 5.2 Data Center Network

The data center network hosts centralized internal services.

Access to servers must be restricted according to business requirements and the principle of least privilege.

### 5.3 DMZ

The DMZ hosts public-facing services and separates externally accessible systems from the internal corporate network.

Traffic between the Internet, DMZ, and internal networks must be controlled through security policies.

### 5.4 Voice and IoT Network

IP phones, printers, scanners, and access control devices must operate in dedicated network segments.

This separation reduces unnecessary communication between infrastructure devices and employee workstations.

### 5.5 Management and Guest Networks

Network management interfaces must be accessible only to authorized IT administrators.

Guest Wi-Fi must provide Internet access without allowing access to internal corporate resources.

## 6. Network Connectivity Between Locations

The Zagreb headquarters and Split branch must communicate securely.

The proposed design includes:

- Site-to-Site IPsec VPN between Zagreb and Split.
- Centralized access to selected services hosted in Zagreb.
- Separate IP addressing ranges for each location.
- Routing between authorized networks at both sites.

The network must also support Remote Access VPN for authorized employees working outside company offices.

Site-to-Site VPN and Remote Access VPN are separate connectivity requirements and will be designed independently.

## 7. Security Requirements

Security is a fundamental requirement of the proposed enterprise network.

The design will follow these principles:

- **Network Segmentation:** Separate departments and infrastructure services using VLANs.
- **Access Control:** Restrict communication between network segments using ACLs and firewall policies.
- **Least Privilege:** Grant users and devices only the access required for their roles.
- **Infrastructure Protection:** Restrict administrative access to network devices.
- **Guest Isolation:** Prevent guest devices from accessing internal company resources.
- **Secure Remote Connectivity:** Use VPN technology for remote and inter-site connections.
- **Infrastructure Separation:** Isolate public-facing services from internal systems.

Additional security mechanisms, including centralized authentication and network access control, may be explored in later project phases.

## 8. Project Scope

This project will cover the design, simulation, configuration, and documentation of a two-location enterprise network.

**Included in the project:**
- Enterprise network topology design.
- IPv4 addressing and subnetting.
- VLAN planning and implementation.
- Inter-VLAN routing.
- Routing between Zagreb and Split.
- Network segmentation and access control.
- Basic infrastructure services.
- VPN concepts and simulated connectivity where supported by the selected devices.
- Connectivity and configuration testing.

**Tools:**
- Cisco Packet Tracer.
- diagrams.net.
- Git and GitHub.

## 9. Design Assumptions and Limitations

This project represents a fictional enterprise environment created for educational and portfolio purposes.

The proposed network design is a simulation and does not represent a production deployment.

The number of network devices, IP addresses, and infrastructure services may be adjusted during the design and implementation phases.

Some enterprise security and VPN capabilities may not be fully supported by Cisco Packet Tracer. Any such limitations will be documented rather than presented as implemented functionality.

## 10. Project Goal

The primary goal is to develop a structured enterprise network design that demonstrates practical knowledge of networking fundamentals, network segmentation, IP addressing, routing, and basic network security.

The final result will include technical documentation, network topology diagrams, simulated device configurations, and connectivity test results.
