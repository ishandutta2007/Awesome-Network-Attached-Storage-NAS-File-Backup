# 💾 Awesome Network Attached Storage (NAS) & File Backup 🛡️

<div align="center">

<img src="./assets/banner.svg" alt="Awesome Network Attached Storage NAS and File Backup Banner" width="100%" />

<a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a><a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?syyle=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-blue.svg)](LICENSE)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/ishandutta2007/Awesome-Network-Attached-Storage-NAS-File-Backup)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/ishandutta2007/Awesome-Network-Attached-Storage-NAS-File-Backup/pulls)
[![Storage Protocols](https://img.shields.io/badge/Protocols-NFS%20%7C%20SMB%20%7C%20S3%20%7C%20iSCSI-orange.svg)](#)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>

<p align="center">
  <b>A curated catalog of enterprise Network Attached Storage (NAS), distributed file backup systems, cloud resilience suites, and open-source file protection engines.</b><br>
  Explore commercial SaaS/hybrid platforms and self-hosted open-source software for immutable backups, deduplication, snapshot management, and petabyte-scale unstructured data resilience.
</p>

🌟 **Star this repository if you find it helpful!** 🌟

</div>

---

## 📑 Table of Contents
- [🌐 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [🏢 SaaS & Enterprise Hosted Platforms](#-saas--enterprise-hosted-platforms)
  - [📊 SaaS & Commercial Platform Comparison Table](#-saas--commercial-platform-comparison-table)
  - [🔍 Deep-Dive: Enterprise Platform Highlights](#-deep-dive-enterprise-platform-highlights)
- [🔓 Open-Source Software & Self-Hosted Backup Engines](#-open-source-software--self-hosted-backup-engines)
  - [⭐ Open-Source Software Comparison Table](#-open-source-software-comparison-table)
  - [🔍 Deep-Dive: Open-Source Tools Overview](#-deep-dive-open-source-tools-overview)
- [⚖️ Architecture Matrix: Protocol & Feature Support](#-architecture-matrix-protocol--feature-support)
- [🤝 Contributing](#-contributing)
- [💖 Support](#-support)
- [⭐ Star History](#-star-history)
- [📄 License](#-license)

---

## 🌐 Sector Overview & Market Dynamics

The global **Network Attached Storage (NAS)** and **Enterprise File Backup / Data Resilience** market represents an estimated **$30B to $50B+ valuation**, driven at a projected compound annual growth rate (**CAGR of ~12% to 15%**) by exponential unstructured data growth (AI training sets, rich media, telemetry) and escalating ransomware defense mandates.

Market structure follows a distinct **two-tier concentration model**:
1. **Enterprise Core & Scale-Out File Tier (Highly Concentrated / Oligopolistic):** Dominated by a consolidated cadre of legacy infrastructure titans (Dell Technologies, NetApp, Pure Storage) and cyber-resilience leaders (Veeam, Commvault, Cohesity, Rubrik) who command high switching barriers through proprietary snapshot engines, deep hardware acceleration, and enterprise compliance guarantees.
2. **SMB, Homelab & Self-Hosted File Protection Tier (Moderately Fragmented):** Highly competitive and collaborative, populated by flexible cloud object stores (Wasabi, Backblaze) and powerful open-source deduplication utilities (Rclone, Restic, BorgBackup, Kopia) addressing localized NAS shares, off-site replication, and cost-optimized sovereign homelabs.

---

## 🏢 SaaS & Enterprise Hosted Platforms

Commercial, managed, and cloud-hosted enterprise NAS data protection platforms, file fabric managers, and cloud storage repositories.

### 📊 SaaS & Commercial Platform Comparison Table

> *Ranked in descending order by parent company scale (Market Cap / Enterprise Valuation / ARR).*

| Product / Vendor | Company Scale (Valuation / Revenue) 📈 | Starting Pricing (Specific Tier) 💰 | Free Tier & Trial Limits ⏳ | Architecture & Protocol Focus 🔌 | Target Workload 🎯 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **[Dell PowerScale (APEX)](https://www.dell.com/en-us/dt/storage/powerscale.htm)** | **$314B+ Market Cap** ($174B+ Rev) | **$100 - $150 / TB** (APEX AWS subscription; base nodes from $11,000/ea) | **No self-service free tier**; 30–60 day sales-assisted lab / PoC evaluation | Scale-Out NAS Appliance, OneFS, NFS, SMB, S3 | Petabyte-scale enterprise unstructured workloads & AI pipelines |
| **[NetApp Cloud Volumes ONTAP](https://www.netapp.com/cloud-services/cloud-volumes-ontap/)** | **$35B Market Cap** ($6B+ Rev) | **$0.05 / TiB / hr** (~$35/TB/mo PAYGO) or $0.034/GB/mo on annual commit | **30-Day Free Trial** (unlimited software features across AWS/Azure/GCP; compute/disk billed by cloud provider) | Cloud-Native NAS Software, ONTAP, NFS, SMB, iSCSI | Enterprise disaster recovery, hybrid replication & cloud file shares |
| **[Pure Storage FlashBlade](https://www.purestorage.com/products/file-and-object/flashblade.html)** | **$16B+ Market Cap** ($3.1B+ Rev) | **$87 / TB / mo** ($0.085/GiB/mo via Evergreen//One UFFO 100 TiB commit) | **No public free tier**; 30-day enterprise evaluation & hardware try-and-buy program | All-Flash Scale-Out NAS / Object, DirectFlash, NFS, SMB, S3 | High-throughput AI/ML, supercomputing & analytics |
| **[Veeam NAS Backup](https://www.veeam.com/solutions/backup-recovery/nas.html)** | **$15B Valuation** ($2B+ ARR) | **$14.00 / TB / mo** (Veeam Data Cloud Vault) / ~$150 / workload / yr | **30-Day Full-Featured Free Trial** (Veeam Data Platform & Vault, full protocol access) | Software-defined Proxy, Snapshot Tracking, CIFS, NFS, NDMP | Unified VM + Enterprise NAS backup with hardware snapshot offload |
| **[Cohesity SmartFiles](https://www.cohesity.com/products/smartfiles/)** | **$17B+ Post-Merger Valuation** ($1.5B ARR) | **$150 / TB / yr** (~$12.50/TB/mo software license for enterprise commit) | **30-Day Free Trial** (via Cohesity DataProtect SaaS; SmartFiles PoC upon request) | Software-defined Unified File/Object, Helios, NFS, SMB, S3 | Cross-volume deduplication, ransomware isolation & multi-tier archiving |
| **[Rubrik NAS Cloud Direct](https://www.rubrik.com/solutions/nas-backup)** | **$14B+ Market Cap** ($1.4B+ Rev) | **$130 / BETB / mo** (Back-End Terabyte 3-yr commit tier) | **30-Day SaaS Trial** (limited to 10 TB backup capacity / 500 users for SaaS workloads) | Cloud Control Plane, Stateless VM, SMB, NFS, Hard Links | Petabyte-scale fast file migration, cloud archiving & rapid disaster recovery |
| **[Commvault File & NAS Backup](https://www.commvault.com/supported-technologies/nas-backup)** | **$6.8B Market Cap** ($1.25B Rev) | **$90 / TB / mo** (Commvault Cloud File/Object SaaS) / $150/FETB/yr software | **30-Day Free Trial** (Commvault Cloud, no credit card required, instant multi-workload access) | SaaS & Hybrid Engine, Air Gap Protect, CIFS, NFS, NDMP, Isilon | Cyber-resilience, automated threat scan & immutable air-gapped protection |
| **[Druva File & NAS Backup](https://www.druva.com/solutions/nas-backup/)** | **$2.0B Valuation** ($200M+ ARR) | **$200 / TB / mo** (SaaS credit model post-deduplication, 1 TB commit) | **30-Day Free Trial** (full self-service cloud portal access, no credit card required) | 100% SaaS Architecture, Stateless NAS Proxy, SMB 3+, NFS v3 | Completely hands-off zero-infrastructure cloud backup for distributed filers |
| **[Wasabi Hot Cloud Storage](https://wasabi.com/cloud-storage-pricing/)** | **$1.8B Valuation** ($120M+ Rev) | **$7.99 / TB / mo** (flat-rate storage with zero egress or API request fees) | **30-Day Free Trial** (up to 1 TB of fully functional S3-compatible cloud storage) | High-Performance S3 Cloud Object Storage Backend | Affordable, immutable secondary repository for NAS offloading & tape replacement |

---

### 🔍 Deep-Dive: Enterprise Platform Highlights

- 🏢 **Dell PowerScale:** Industry-leading scale-out architecture featuring the OneFS distributed file system, SmartDedupe, and SmartLock WORM policy compliance for petabyte-scale data lakes.
- ☁️ **NetApp Cloud Volumes ONTAP:** Software-defined multi-cloud NAS delivering native ONTAP snapshots, thin provisioning, block-level deduplication, and automated cloud tiering across AWS, Azure, and Google Cloud.
- ⚡ **Pure Storage FlashBlade:** The flagship all-flash platform for unstructured file and object data, delivering up to 650 GB/s throughput, DirectFlash efficiency, and Evergreen non-disruptive upgrades.
- 🔄 **Veeam NAS Backup:** Uses intelligent Windows/Linux file proxies alongside vendor-native change tracking (NetApp ONTAP, Dell PowerScale, Nutanix Files) to accelerate incremental backup windows without full rescans.
- 🛡️ **Cohesity SmartFiles:** Consolidates unstructured silos under a single software-defined namespace, offering ML-driven anomaly detection, anti-ransomware immutability, and 96x data reduction ratios.
- 🚀 **Rubrik NAS Cloud Direct:** Employs stateless distributed virtual machines deployed adjacent to physical NAS arrays to ingest and copy petabytes of SMB/NFS data without local cache consumption.
- 🔒 **Commvault File & NAS Backup:** Enterprise data defense suite with broad protocol coverage (NDMP, CIFS, NFS), metallic cloud air-gapping, inline anomaly analytics, and deep file indexing.
- ☁️ **Druva File & NAS Backup:** Cloud-native architecture utilizing lightweight auto-discovering proxies to stream compressed, deduplicated file trees directly into AWS S3 cold and warm tiers.
- 📦 **Wasabi Hot Cloud Storage:** Low-cost S3-compliant target pricing eliminating egress and API call penalties, ideal for secondary NAS copies and compliance archiving.

---

## 🔓 Open-Source Software & Self-Hosted Backup Engines

Self-hosted, community-driven backup software, sync engines, and deduplicating tools for protecting NAS shares, homelabs, and on-premises storage arrays.

### ⭐ Open-Source Software Comparison Table

> *Ranked in descending order by GitHub community popularity (Stargazers count).*

| Project | GitHub Stars 🌟 | Primary Stack 🛠️ | License 📜 | Deduplication & Security 🔐 | NAS Target Support 📁 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **[Rclone](https://github.com/rclone/rclone)** | [![Stars](https://img.shields.io/github/stars/rclone/rclone?style=social&color=white)](https://github.com/rclone/rclone/stargazers) | Go | MIT | Hash verification, chunker, rclone crypt (AES-256) | S3, WebDAV, SFTP, SMB, NFS, 70+ Cloud providers |
| **[Restic](https://github.com/restic/restic)** | [![Stars](https://img.shields.io/github/stars/restic/restic?style=social&color=white)](https://github.com/restic/restic/stargazers) | Go | BSD-2-Clause | Content-defined chunking (CDC), AES-256 encryption | Local NAS, SFTP, REST server, AWS S3, MinIO, B2 |
| **[Duplicati](https://github.com/duplicati/duplicati)** | [![Stars](https://img.shields.io/github/stars/duplicati/duplicati?style=social&color=white)](https://github.com/duplicati/duplicati/stargazers) | C# / .NET | LGPL-2.1 | Block-level deduplication, AES-256 encryption, Web GUI | SMB, WebDAV, FTP, SFTP, S3, Google Drive, Backblaze |
| **[Kopia](https://github.com/kopia/kopia)** | [![Stars](https://img.shields.io/github/stars/kopia/kopia?style=social&color=white)](https://github.com/kopia/kopia/stargazers) | Go | Apache-2.0 | Content-addressed chunking, compression (zstd), end-to-end encryption | Local/Mounted NAS paths, WebDAV, SFTP, S3, Azure Blob, GCS |
| **[BorgBackup](https://github.com/borgbackup/borg)** | [![Stars](https://img.shields.io/github/stars/borgbackup/borg?style=social&color=white)](https://github.com/borgbackup/borg/stargazers) | Python / C | BSD-3-Clause | Variable-block deduplication, authenticated encryption (AES-CTR/HMAC) | Local mount, SSH/Remote repository, Synology/QNAP shell |
| **[OpenZFS](https://github.com/openzfs/zfs)** | [![Stars](https://img.shields.io/github/stars/openzfs/zfs?style=social&color=white)](https://github.com/openzfs/zfs/stargazers) | C | CDDL-1.0 | Native block deduplication, copy-on-write snapshots, ZFS send/recv | Native enterprise NAS foundation (TrueNAS, Proxmox, Linux) |
| **[OpenMediaVault](https://github.com/openmediavault/openmediavault)** | [![Stars](https://img.shields.io/github/stars/openmediavault/openmediavault?style=social&color=white)](https://github.com/openmediavault/openmediavault/stargazers) | PHP / Python | GPL-3.0 | Rsync, snapshot plugins, scheduled backup tasks, full Web UI | Debian-based DIY NAS, SMB/CIFS, NFS, rsync, FTP |
| **[TrueNAS Middleware](https://github.com/truenas/middleware)** | [![Stars](https://img.shields.io/github/stars/truenas/middleware?style=social&color=white)](https://github.com/truenas/middleware/stargazers) | Python / C | BSD-2-Clause | ZFS snapshots, native replication, Cloud Sync (Rclone integration) | Enterprise ZFS storage OS, SMB, NFS, iSCSI, S3, NVMe-oF |
| **[Vorta](https://github.com/borgbase/vorta)** | [![Stars](https://img.shields.io/github/stars/borgbase/vorta?style=social&color=white)](https://github.com/borgbase/vorta/stargazers) | Python / PyQt | GPL-3.0 | Borg-backed variable deduplication, client-side encryption | Desktop/Server client connecting to Borg repos on remote NAS |
| **[Restic REST Server](https://github.com/restic/rest-server)** | [![Stars](https://img.shields.io/github/stars/restic/rest-server?style=social&color=white)](https://github.com/restic/rest-server/stargazers) | Go | BSD-2-Clause | Append-only mode protects repositories from ransomware deletion | High-performance HTTP server deployable directly onto NAS |
| **[Bareos](https://github.com/bareos/bareos)** | [![Stars](https://img.shields.io/github/stars/bareos/bareos?style=social&color=white)](https://github.com/bareos/bareos/stargazers) | C++ / Python | AGPL-3.0 | Volume encryption, software deduplication plugin, SQL catalog | Enterprise client-server daemon, NDMP, Tape, Disk, S3 |
| **[SDFS Deduplication FS](https://github.com/opendedup/sdfs)** | [![Stars](https://img.shields.io/github/stars/opendedup/sdfs?style=social&color=white)](https://github.com/opendedup/sdfs/stargazers) | Java / C | Apache-2.0 | Inline block deduplication (up to 95% reduction), cloud tiering | POSIX filesystem for backup targets, iSCSI, NFS |
| **[Packrat](https://github.com/jvinet/packrat)** | [![Stars](https://img.shields.io/github/stars/jvinet/packrat?style=social&color=white)](https://github.com/jvinet/packrat/stargazers) | Shell / Perl | GPL-2.0 | dar-based incremental archives, symmetric encryption | Tar/Dar incremental backups to S3, FTP, SSH & NAS |

---

### 🔍 Deep-Dive: Open-Source Tools Overview

#### 1. [Rclone](https://github.com/rclone/rclone)
- **Description:** Known as the *"Swiss army knife of cloud storage"*, Rclone syncs files and directories to and from local NAS devices, remote filers, and over 70 cloud object storage providers.
- **Key Capabilities:** Bidirectional synchronization, bandwidth limiting, on-the-fly encryption (`rclone crypt`), virtual filesystem mounting (`rclone mount`), and parallel multi-threaded transfers.
- **Best For:** Automating off-site replication from local NAS arrays (Synology, QNAP, TrueNAS) to low-cost cloud targets (Wasabi, Backblaze B2, S3).

#### 2. [Restic](https://github.com/restic/restic)
- **Description:** Fast, secure, and modern backup program packaged as a standalone binary in Go, utilizing cryptography and content-defined chunking.
- **Key Capabilities:** Fast incremental snapshots, deduplication across files and revisions, AES-256 encryption with Poly1305 MAC, and native support for local storage, SFTP, HTTP REST server, and cloud buckets.
- **Best For:** Small-to-medium server backups and NAS directories requiring zero administrative overhead and cryptographically verified integrity.

#### 3. [Duplicati](https://github.com/duplicati/duplicati)
- **Description:** User-friendly backup client featuring a built-in browser-based administration UI, scheduling wizard, and cross-platform compatibility.
- **Key Capabilities:** AES-256 encrypted block chunking, incremental changes, bandwidth throttling, and cloud connectors for Google Drive, OneDrive, Amazon S3, and local CIFS/NFS mounts.
- **Best For:** Homelabbers and SMB desktop/NAS administrators wanting an intuitive web interface without managing CLI configuration scripts.

#### 4. [Kopia](https://github.com/kopia/kopia)
- **Description:** Advanced backup engine offering both a feature-packed CLI and an Electron-based desktop GUI, built in Go for speed and concurrency.
- **Key Capabilities:** Content-addressable variable chunking, selectable compression algorithms (zstd, s2), robust snapshot retention policies, multi-user repository locking, and fast file indexing.
- **Best For:** Power users and distributed environments seeking blazing snapshot performance and snapshot scheduling.

#### 5. [BorgBackup (Borg)](https://github.com/borgbackup/borg)
- **Description:** Industry benchmark for deduplicating archiver on Unix-like operating systems.
- **Key Capabilities:** Variable-block deduplication based on Rabin fingerprinting, authenticated encryption, data integrity checks, and direct mounting of backup archives as FUSE filesystems for granular file restoration.
- **Best For:** Linux workstations, servers, and dedicated NAS nodes with SSH access seeking maximum data compression and storage reduction.

#### 6. [OpenZFS](https://github.com/openzfs/zfs)
- **Description:** Advanced enterprise-grade file system and volume manager with copy-on-write mechanics, self-healing data integrity verification, and instant snapshot capabilities.
- **Key Capabilities:** Native dataset encryption, ZFS send/receive for instant block replication between storage pools, RAID-Z resiliency, and inline compression (LZ4/ZSTD).
- **Best For:** Constructing robust physical storage layers, powering enterprise NAS distributions, and disaster-proof local snapshot architectures.

#### 7. [TrueNAS](https://github.com/truenas/middleware) & [OpenMediaVault](https://github.com/openmediavault/openmediavault)
- **Description:** Dedicated NAS operating system distributions providing web-based appliance interfaces for disk management, share provisioning, and automated backup routines.
- **Key Capabilities:** Centralized SMB/NFS share management, integrated snapshot replication pipelines, user permission modeling, and Docker/Kubernetes container orchestration.
- **Best For:** Converting commodity hardware or purpose-built servers into fully managed Network Attached Storage servers.

---

## ⚖️ Architecture Matrix: Protocol & Feature Support

| Solution | Protocol Coverage | Deduplication Type | Immutability / Ransomware Defense | Deployment Model |
| :--- | :--- | :--- | :--- | :--- |
| **Dell PowerScale** | NFS v3/v4, SMB 3.x, S3, HDFS, NDMP | Global Post-Process (SmartDedupe) | SmartLock WORM & Cyber Recovery Vault | Physical Appliance / Cloud Marketplace |
| **NetApp CVO** | NFS, SMB, iSCSI, NVMe | Inline & Background Block Level | NetApp SnapLock & Immutable Snapshots | Cloud-Hosted VM (AWS / Azure / GCP) |
| **Pure FlashBlade** | NFS v3/v4.1, SMB 2.1/3, S3 | Inline Hardware-Accelerated | SafeMode Immutable Snapshots | All-Flash Modular Hardware / STaaS |
| **Veeam** | CIFS/SMB, NFS, Storage Snapshot APIs | Source & Target Side Deduplication | S3 Object Lock & Hardened Linux Repo | Self-Managed Software / SaaS Cloud Vault |
| **Cohesity** | NFS, SMB, S3 API | Global Distributed Variable Block | DataLock WORM & ML Anomaly Detection | Hardware Cluster / Software-Defined SaaS |
| **Rubrik** | SMB, NFS, POSIX Filesystem | Inline Distributed Block Deduplication | Append-Only Atlas File System | Stateless Virtual Appliance + Cloud Plane |
| **Commvault** | NDMP, CIFS, NFS, S3 | Source-side & Global Deduplication | Air Gap Protect & Isolated Cloud Tiers | SaaS Service / Managed Software |
| **Druva** | SMB 3+, NFS v3 | Global Client-Side Deduplication | Cloud-Isolated S3 Immutability | Fully Managed Zero-Infra SaaS |
| **Wasabi** | S3 API (100% bit-compatible) | Underlying Object Storage Management | S3 Object Lock (Compliance & Governance) | Managed Hot Cloud Storage |
| **Rclone** | 70+ Backends (S3, SMB, WebDAV, SFTP) | Chunker / Hash Matching | Cloud Provider Object Lock Integration | Lightweight Single Binary CLI |
| **Restic** | Local, SFTP, REST Server, S3 | Content-Defined Chunking (CDC) | Append-Only REST Server Mode | Single Binary CLI / Daemon |
| **Kopia** | Local, S3, WebDAV, SFTP | Content-Addressed Chunking | Repository Locking & Snapshot Retention | Single Binary CLI / Desktop GUI |
| **BorgBackup** | Local Path, SSH Remote Server | Rabin-based Variable Chunking | Read-Only Append Mode via SSH ForceCommand | Python/C CLI |
| **OpenZFS** | Block Device / Local POSIX VFS | In-Pool Block Deduplication & Compression | Read-Only Snapshots & Clones | Kernel Module / Core Filesystem |

---

## 🤝 Contributing

Contributions to this directory are encouraged! If you maintain or rely on an enterprise-grade or open-source NAS backup solution that is missing from this compilation, please submit a pull request:

1. Fork this repository 🍴
2. Add your product or open-source tool to the appropriate section:
   - Provide software name, project repository URL, license, and brief overview.
   - For open-source tools, include the GitHub stars social badge linked to its `/stargazers` page.
   - For commercial/SaaS tools, supply verifiable starting tier pricing and explicit trial periods.
3. Verify that the table formatting is clean and properly aligned.
4. Submit your pull request with a descriptive title! 🚀

---

## 💖 Support

Thank you for exploring and supporting this curated resource! 🌟 If this directory has helped you discover, evaluate, or deploy storage and backup tools for your infrastructure, please consider supporting the project:

- ⭐ **Star this repository** to improve visibility and help other DevOps/SysAdmin practitioners find it!
- 🍴 **Fork the repo** to contribute new tools, updates, or benchmark insights.
- 📢 **Share it** with fellow storage engineers, homelab hobbyists, and cloud architects on Discord, Reddit, or X.
- ☕ **Buy me a coffee / Sponsor**: If you appreciate this work and want to support ongoing maintenance and new curated resources, check out my [GitHub Sponsor Dashboard](https://github.com/sponsors/ishandutta2007). Your support is deeply appreciated!

---

##  Star History
[![Star History Chart](https://www.star-history.com/svg?repos=ishandutta2007/Awesome-Network-Attached-Storage-NAS-File-Backup&type=date&legend=top-left)](https://www.star-history.com/#ishandutta2007/Awesome-Network-Attached-Storage-NAS-File-Backup&type=date&legend=top-left)

---

## 📄 License

This repository and curated compilation are released under the [Creative Commons Zero v1.0 Universal License (CC0 1.0)](LICENSE). Project trademarks, badges, and brand assets are the property of their respective owners.

<div align="center">
  <sub>Built with ❤️ for storage engineers, system administrators, and homelab builders worldwide.</sub>
</div>
