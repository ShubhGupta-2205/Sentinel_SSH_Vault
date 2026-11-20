Sentinel SSH Secure Vault

An offline-first encrypted file vault for Linux with integrated authentication brute-force analysis, security monitoring, and owner controls.







Sentinel SSH Secure Vault is a Linux desktop application designed to protect personal files behind a master password while providing integrated authentication monitoring and brute-force analysis.

Sentinel combines encrypted file storage, failed-authentication tracking, security analytics, vault integrity verification, and owner security controls into a single application.

The project is designed with an offline-first approach: your vault and security data remain local, without requiring cloud accounts or external telemetry.

Features

🔐 Encrypted File Vault

Protect files using a master password.

Encrypt imported files using AES-GCM authenticated encryption.

Import individual files or entire folders.

Open and export files when authenticated.

Delete individual files or clear the vault.

Change the vault password.

Keep imported originals untouched.

Store encrypted objects separately from the original files.

🛡️ Authentication Brute-Force Analyzer

Sentinel monitors authentication attempts against its own vault.

Record failed unlock attempts.

Record successful authentication events.

Timestamp security events.

Track repeated authentication failures.

Detect consecutive failed attempts.

Maintain authentication incident history.

Record lockout events.

Display authentication activity in the analyzer.

Monitor local vault authentication events.

View success and failure statistics.

View event activity over time.

Analyze authentication incidents.

The analyzer is integrated into Sentinel's security area rather than operating as a separate application.

📊 Security Overview

The security overview provides a centralized view of the vault and its security-related information.

Authentication statistics.

Failed and successful unlock events.

Vault status.

Encrypted storage information.

Lockout configuration.

Monitoring status.

Local security information.

Statistics are derived from locally recorded events. Simulated events are clearly distinguished from real authentication events.

🔎 Vault Integrity Verification

Sentinel includes a vault integrity verification feature that checks encrypted objects by attempting to authenticate and decrypt them in memory.

It can help identify:

Corrupted encrypted objects.

Objects that fail cryptographic verification.

Integrity-related problems with stored vault data.

📋 Owner Audit Trail

Security-relevant owner actions can be recorded in an encrypted audit history.

Examples include:

File imports.

File exports.

File deletion.

Password changes.

Integrity scans.

Other selected vault operations.

The audit history is protected using the vault encryption key.

🚨 Lockout Protection

Sentinel includes a failed-authentication protection mechanism.

Configurable failed-attempt threshold.

Temporary lockout after repeated failures.

Lockout duration.

Persistent lockout state across application restarts.

Failed-attempt incident logging.

Lockout event history.

The default policy is five failed attempts followed by a 60-second lockout.

🎨 Blackwater Edition

Version 3.2.0 introduces the Blackwater visual direction:

Near-black interface.

Graphite panels.

Restrained blue accents.

Clear security-status indicators.

Dark desktop-oriented interface.

Integrated security navigation.

Supported Systems

Sentinel is designed for Debian-based Linux distributions.

Tested or intended platforms include:

Debian

Ubuntu

MX Linux

The application is distributed as a Debian .deb package.
