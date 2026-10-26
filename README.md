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

---

## Week 2 — Detection Engineering and Security Monitoring

In Week 2, I expanded the Mini-SOC with advanced monitoring and detection capabilities:

- **Custom Wazuh Rules:** Developed LabShop authentication detection and brute-force correlation rules.
- **File Integrity Monitoring:** Detected file and registry changes on Ubuntu and Windows.
- **Suricata IDS:** Integrated network intrusion detection with Wazuh using custom signatures.
- **Security Assessment:** Performed CIS benchmark assessments and vulnerability analysis, including Ubuntu security remediations.
- **Backup and Recovery:** Preserved configurations and created VMware snapshots for all three VMs.

## Week 2 Report

📄 [**Download the Week 2 Technical Report (Word)**](Week%202%20Mini-SOC%20in%20a%20Box%20Report.docx)

---

**Note:** GitHub may not preview large `.docx` files. Download the reports to view the complete documentation, configuration steps, test results, and embedded screenshots.
