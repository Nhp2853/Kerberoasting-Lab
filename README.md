# Kerberoasting-Lab
“Simulating Kerberoasting in a containerized environment with cloud and GRC security context”
# Kerberoasting Lab (Kuberroasting Style)

This project simulates a Kerberoasting attack in a containerized lab environment using Docker, Kali Linux, and Impacket. It also demonstrates how governance failures in identity management create opportunities for credential-based attacks — even in hybrid or cloud environments.

---

## Lab Setup

- **Attacker**: Kali Linux VM
- **Target**: Docker container simulating a Kerberos environment
- **Tools**: Docker, Impacket, Hashcat, Linux
- **Environment**: Fully containerized, GRC-aware

---

## Attack Flow (To Be Demonstrated)

1. Enumerate SPNs from victim (using Impacket)
2. Request TGS tickets
3. Extract & save Kerberos ticket hashes
4. Crack offline with Hashcat
5. Show lateral movement or access escalation

---

## Project Structure

| Folder | Purpose |
|--------|---------|
| `/attack-guide/` | Step-by-step commands used in the lab |
| `/ppt/` | Final LinkedIn presentation slides |
| `/screenshots/` | Screenshots from Kali and Docker attack simulation |
| `report.md` | Governance & framework mapping (NIST, MITRE, CIS, etc.) |

---

## GRC + Cloud Security Tie-In

This lab highlights the intersection of offensive techniques and GRC breakdowns:
- Weak credential policies (NIST IA-5, CIS 4.8)
- Poor service account governance (NIST AC-2, CSF PR.AC-1)
- Inadequate monitoring (NIST SI-4, CSF DE.CM-3)
- Real-world threat mapping (MITRE ATT&CK T1558.003 – Kerberoasting)

---

### Status: *In Progress*

- [x] PowerPoint slides created (to be uploaded in `/ppt`)
- [ ] Lab attack executed and screenshots saved
- [ ] Report finalized and added
