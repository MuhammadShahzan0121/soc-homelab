# Wazuh ARM Compatibility Issue

## Problem Encountered

While attempting to install Wazuh on the Ubuntu VM, the installation failed due to system architecture incompatibility.

Error Message:

```text id="1m4v8x"
This script must be run on a 64-bit system
```

---

## Investigation

The system architecture was checked using:

```bash id="0q7m2n"
uname -m
```

Result:

```text id="9v2t4m"
aarch64
```

This confirmed the VM was running ARM64 architecture on Apple Silicon hardware.
<img width="657" height="488" alt="arm64-check" src="https://github.com/user-attachments/assets/cd85f164-e242-4c08-a589-8602382f5e69" />
Uploaded ARM architecture screenshot
---

## Resolution

The lab design was updated to use Elasticsearch, Kibana and Winlogbeat because it provides better compatibility with ARM-based environments.

---

## Lessons Learned

* Apple Silicon Macs commonly use ARM64 virtual machines.
* Software compatibility should always be checked before deployment.
* Troubleshooting compatibility issues is an important cybersecurity skill.
