# Security Policy

## Repository Classification

**Public Repository - Intentionally Public**

This repository is intentionally public as it serves as the distribution point for Ferentin CLI releases. Users download CLI binaries from this repository.

### What This Repository Contains

- Pre-built CLI binaries for various platforms (macOS, Linux, Windows)
- Release artifacts and checksums
- Installation instructions

### What This Repository Does NOT Contain

- Source code for the CLI application
- API keys, secrets, or credentials
- Internal configuration or infrastructure details
- Customer data or personally identifiable information (PII)

## Security Controls

### Binary Integrity

- All releases include SHA256 checksums for verification
- Binaries are built from the private source repository via CI/CD
- Release artifacts are immutable once published

### Verification

Users can verify downloaded binaries:

```bash
# Download the checksum file
# Verify the binary matches the checksum
sha256sum -c ferentin-cli_<version>_checksums.txt
```

## Reporting Security Vulnerabilities

We take security seriously. If you discover a security vulnerability, please report it responsibly.

### How to Report

**DO NOT** create a public GitHub issue for security vulnerabilities.

Instead, please email: **security@ferentin.net**

Include:
- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Any suggested remediation

### Response Timeline

- **Acknowledgment**: Within 48 hours
- **Initial Assessment**: Within 5 business days
- **Resolution Timeline**: Depends on severity, typically 30-90 days

### Scope

This security policy covers:
- CLI binaries distributed through this repository
- The installation and update process

For vulnerabilities in the Ferentin platform itself, please contact security@ferentin.net.

## SOC 2 Compliance

This repository is documented as an **intentional exception** in Ferentin's SOC 2 compliance program:

- **Justification**: Required for public CLI distribution
- **Compensating Controls**: No source code or secrets, checksums for integrity verification
- **Review Frequency**: Quarterly

## Contact

- **Security Issues**: security@ferentin.net
- **General Support**: support@ferentin.net
- **Documentation**: https://docs.ferentin.net

---

**Last Review**: January 2026
**Next Review**: April 2026
