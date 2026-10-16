
# Mini-SOC in a Box

A hands-on Blue Team project focused on building and operating a small, isolated Security Operations Center (SOC).

## Week 1 — Build the Lab and Deploy Wazuh

In Week 1, I set up a three-VM lab using VMware Workstation Pro:

- **siem-host:** Ubuntu Server running Wazuh 4.14.8 (Manager, Indexer, and Dashboard) in Docker.
- **ubuntu-web:** Ubuntu Server with Apache and a Wazuh agent.
- **win-client:** Windows 10 with a Wazuh agent and Sysmon.

The lab uses a host-only network, synchronized clocks, and controlled network access.

I verified centralized monitoring with five security test events:
1. Failed SSH login
2. Successful `sudo` command
3. New Linux user creation
4. Windows process creation (Sysmon)
5. Failed Windows login

## Week 1 Report

📄 [**Download the Week 1 Technical Report (Word)**](Week%201%20Mini-SOC%20in%20a%20Box%20Report.docx)

> **Note:** GitHub may not preview large `.docx` files. Download the report to view the complete documentation, architecture diagram, test results, and embedded screenshots.
