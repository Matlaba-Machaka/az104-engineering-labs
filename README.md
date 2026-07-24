# Azure-Administrator-AZ-104-Lab-Portfolio
Welcome to my AZ-104 exam preparation and engineering portfolio. This repository contains the architecture diagrams, technical configurations, and automation scripts developed during my dedicated hands-on lab phase. Every project here maps directly to the official Microsoft exam objectives.


## 🛠️ Portfolio Overview & Exam Mapping

| Project | Focus Domain | Key Azure Services Used |
| :--- | :--- | :--- |
| **[Project 1](./project-1-hybrid-networking)** | Configure & Manage Virtual Networking | Azure Firewall, VNet Peering, UDR, App Gateway |
| **[Project 2](./project-2-compute-storage)** | Deploy & Manage Compute + Storage | VMSS, Availability Zones, Azure Files, SMB |
| **[Project 3](./project-3-identity-governance)** | Manage Azure Identities & Governance | Entra ID, Custom RBAC (JSON), Azure Policy, Locks |
| **[Project 4](./project-4-iac-automation)** | Infrastructure as Code Automation | Bicep, ARM Templates (JSON), Azure CLI / PowerShell |
| **[Project 5](./project-5-backup-dr)** | Monitor & Back Up Azure Resources | Recovery Services Vault, Backup Policies, File Restore |
| **[Project 6](./project-6-monitoring-alerts)** | Centralized Monitoring & Analytics | Log Analytics Workspace, KQL, Azure Monitor Alerts |

---

## 🚀 Projects Technical Summary

### 1. Secure Hybrid Infrastructure (Networking)
* **Objective:** Establish a highly secure hub-and-spoke network topology with centralized traffic inspection.
* **Core Tasks:** Configured VNet peerings with gateway transit, deployed Azure Firewall with specific network/application rules, and forced all spoke outbound traffic through the firewall using User Defined Routes (UDRs).

### 2. Highly Available Compute Scale Sets (Compute/Storage)
* **Objective:** Design an elastic, zone-redundant web application layer with centralized shared storage.
* **Core Tasks:** Deployed a Virtual Machine Scale Set (VMSS) across multiple Availability Zones, configured dynamic autoscale metrics based on CPU thresholds, and mounted a persistent Azure Files share across all instances via SMB.

### 3. Enterprise Governance & RBAC (Identity)
* **Objective:** Implement a zero-trust governance model using identity boundaries and operational compliance rules.
* **Core Tasks:** Created custom multi-tenant RBAC roles via JSON to restrict VM deletion, enforced regional resource boundaries via Azure Policy, and protected critical data stores using `CanNotDelete` resource locks.

### 4. Infrastructure as Code (IaC) Automation
* **Objective:** Transition from manual portal configurations to declarative, repeatable code deployments.
* **Core Tasks:** Wrote modular Bicep and ARM template files to provision interconnected compute, network, and storage assets, executing them via idempotent Azure CLI and PowerShell scripts.

### 5. Enterprise Backup & Disaster Recovery (Data Protection)
* **Objective:** Protect corporate cloud data against operational failures, accidental deletion, and ransomware.
* **Core Tasks:** Configured a Recovery Services Vault with tailored retention schedules, optimized data replication (LRS transition), and executed live item-level recovery actions back to a running virtual machine.

### 6. Centralized Monitoring, Alerting, and Log Analytics
* **Objective:** Achieve full operational visibility and proactive alerting across cloud-native infrastructure.
* **Core Tasks:** Connected resources to a central Log Analytics Workspace using the Azure Monitor Agent (AMA), extracted real-time performance insights using Kusto Query Language (KQL), and set up automated metric alerts with email action groups.

---

