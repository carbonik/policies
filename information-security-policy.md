# Information Security Policy

## Policy Statement

This policy addresses Carbonik (Hong Kong) Limited ("Carbonik") protection of all data and information.

This policy reasonably adheres to industry standard and best practice and resonably provides safeguards against accident or unlawful destruction, loss, alteration or unauthorized disclosure or access to covered data. It is designed to provide a consistent application of security policy and controls for Carbonik and all Carbonik clients. Customization of these policies on a per-client basis is generally not allowed, except for product security control configurations that can be customized, often by the client, to client needs.

Protection of Carbonik proprietary software and other managed systems shall be addressed to ensure the continued availability of data, systems, and applications to all authorized parties, and to ensure the integrity and confidentiality of impacted data and configuration controls.

As with all Carbonik policies, failure of Carbonik personnel to follow the policy requirements shall result in disciplinary action, up to and including termination.

## Ownership and Administration

This Information Security Policy is owned and administered by Carbonik DevOps Team.

## Applicability

This policy applies to all systems, including network equipment and communication systesm, supporting Carbonik internal and remote operations and products and services. These policies will be reviewed at least once per calendar year and updated to meet currenct best practice.

Carbonik uses reasonable efforts to protect the security and privacy of all information received by, through or on behalf of Carbonik. In cases where a system or provider cannot meet these requirements, exceptions will be noted and documented by DevOps team, and alternative controles will be implemented.

## Security Policies

### Security Awareness, Vulnerabilities, Weaknesses, Events, and Incident Policy

1. Security awareness training shall be conducted at least once per calendar year. Training shall cover information security policies, as well as best practice.
1. Security awareness training shall be given at the first onboarding session for new employees
1. Identified security weakness or security vulnerabilities shall be immediately reported to the DevOps team
1. At no time shall an attempt to be made to take advantage of any security weakness or security vulnerabilities
1. Security weakness or vulnerabilieis that have been compromised will trigger a Security Event. Security Events shall be analyzed by the DevOps team to determine whether they are considered Security Incidents, which are required to be addressed.    

### Identity and Access Management Policy

#### Access Control

1. Establish process for linking all access to system components to each individual users
2. Access to databases shall always be authenticated

#### Account Management

1. Account creation should be reviewed and performed by DevOps team
1. User accounts and access rights for are to be reviewed periodically
1. Upon user role changes, access rights must be modified in a timely manner to reflect the new role
1. Any accounts that have not been accessed within a defined period of time will be disabled
1. Accounts must be disabled and/or deleted in a timely manner following employment termination

#### Privileged Access

1. Personnel with privileged access accounts must refrain from abuse of privilege and must only perform the tasks required to complete their job function

#### Authentication

1. Personnel are required to maintain the confidentiality of personal authentication information
1. All group/shared authentication information must be maintained solely among the authorized members of the group
1. All password must be constructed and implemented according to the minimum requirements of the corresponding system
1. If the security of a password is in doubt, the password should be changed immediately

#### Remote Access

1. All remote access connections to Carbonik networks will be made through the approved remote access method

### Endpoint Security Policy

1. Users shall shutdown, logout or lock workstations when leaving them for any length of time.
1. It is recommended that workstations be restarted at minimum once every 2 weeks.
1. Workstations shall adhere to Virus and Malware Protection Policy.

### Patch Management Policy

1. Server operating systems shall be patched within 30 days of a critical and/or security patch release.
1. Workstations shall be patched within 30 days of a critical and/or security patch release.

### Virus and Malware Protection Policy

1. Up to date anti-virus software for detecting, removing, and protecting against suspected viruses shall be installed on all servers and workstations.
1. Anti-virus software shall be updated regularly for all servers and workstations with the latest anti-virus patches and/or signatures, where applicable.
1. Users shall be made aware of current anti-virus procedures and policies
1. Personnel shall inform the DevOps Team immediately in the event of a possible virus infection
1. Upon notification of a virus infection, systems shall be isolated from the network, scanned, and cleaned appropriately. Any removable media or other systems to which the virus shall have spread shall be treated accordingly.
1. If a system has been identified as potentially infected and removal/quarantine of the virus/malware cannot be definitely proven, the system shall be completely wiped and re-provisioned.

### Network Security Policy

1. Access to internal network services shall be controlled through:
    - Firewall policies, or equivalent
    - Security groups, or equivalent
    - IP whitelists, or equivalent
1. Firewalls or equivalent access controls, shall be used to regulate network traffic for connections to/from the internet or other external networks, as follow:
    - Access control policy shall limit inbound and outbound traffic to only necesary protocols, ports, and/or destinations
    - All inbound internet traffic shall terminate in a DMZ
    - Only DevOps approved connections shall be allowed into Carbonik network
    - The uses of all services, protocols, and ports allowed to access Carbonik networks shall be reviewed on a periodic basis, for approriate usage and control implementation
    - All internet facing rule set modifications shall be reviewed and approved by the DevOps prior to implementation
1. Network intrusion detection systems shall be implemented and monitored by DevOps
1. Secure, encrypted VPN connections to networks not controlled by Carbonik, when required, shall be approved and setup by the DevOps team.

### Data Protection and Encryption Policy

1. To provide data confidentiality in the event of accidental or malicious data loss, all Client data shall be encrypted at rest
1. Strong cryptography and security protocols are required to safe guard Client data during transmission
1. Client data shall not be stored on equipment that is not owned or managed by Carbonik

### Information Lifecycle Policy

#### Collecting

1. Collection of data should be minimized to the amount necessary to support the regular operation

#### Storing

1. Store information in repositories that cannot be accessed by unauthorized individuals
1. Data should be encrypted at rest where reasonable to do so, preferably using technologies like whole disk encryption that is native to the operating system.
1. Limit the number of copies of data to the minimum possible and do not retain longer than needed
1. Portable media (CD-ROMs, USB keys) should not be used to store data

#### Accessing and Sharing

1. Apply the Principle of Least Privilege to all data: Grant access and share data only as needed for an individual or system to perform a required function. Increase scrutiny of these controls as the sensitivity of the data increases.  Ensure processes are in place to immediately remove access upon change in affiliation of any individual.

#### Transmission

1. Encryption should be used during transmission whenever possible.
1. Encryption in transit is strongly recommended
1. Avoid transmitting data via email by sharing files from cloud services instead

#### Destroying

1. Remove the data as soon as it is no longer needed

### Software Development Life Cycle Policy

The following phases must be addressed and incorporated in a consistent manner when developing software. Developers may take necessary adaptations based on the size and complexity of the projects.

#### Phase 1: Defining Scope of Development

1. Anaylzes client information needs. Describe the desired features and operations. Address additional requirements like security.
1. Estimated the required workload.
1. Communicate with client the scope of development and schedule.

#### Phase 2: Development and Testing

1. Development/Testing and production environment shall be reasonably segregated
1. Develop all web applications based on secure coding best practice. Cover, at a minimum, prevention of common OWASP Top 10 coding vulnerabilities in development process. See https://owasp.org/www-project-top-ten/
1. Write test cases to cover core calculation logic
1. Manage all code through version control system to allow viewing of change history and content

#### Phase 3: Deployment

1. Committed source code will be processed by Deployment Pipeline, and only source code that passed all test cases will be available for deployment
1. All deployments must be done with Deployment Pipeline. Manually record deployment when there is no internet connection

- monitoring
- corrective action
- approval/review records, name + date


---


### Backup Policy

### Auditing, Logging and Monitoring Policy

### Audit and Assessments Policy