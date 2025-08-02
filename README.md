
# Hospital Network Simulation (Cisco Packet Tracer)

A self-contained Packet Tracer lab that shows how a mid-size hospital can secure and streamline its IT infrastructure with VLAN segmentation and inter-VLAN routing.

## Why this project exists
Healthcare facilities juggle confidential patient data, time-critical communications and a rapidly growing number of devices. This simulation offers a clean reference architecture you can imitate or extend in your own labs.

## What’s inside
| Component | Purpose |
|-----------|---------|
| **Core + Access switches** | Provide Layer-2 segmentation, trunking and redundancy |
| **Router-on-a-Stick** | Handles inter-VLAN routing for clinical, admin and guest networks |
| **Servers (EMR, DB, Backup)** | Represent business-critical apps that demand low latency |
| **Endpoints** | PCs, laptops, printers and wireless clients placed in typical hospital zones |
| **Security hardening** | SSH-only device access, strong console passwords and basic ACL examples |

## Quick Start
1. Install **Cisco Packet Tracer 8.2** or later.  
2. Clone/download this repo and open `Hospital_Cisco_Packet.pkt`.  
3. Switch from **Realtime → Simulation** to watch ARP, DNS and application traffic flow.  
4. Try a few tests:  
   * From a “Doctor PC”, ping the EMR server IP.  
   * From a “Guest Wi-Fi” client, verify you can’t reach the database server (inter-VLAN ACL).  
5. Tweak configs to experiment—key devices have annotated startup banners.

## Learning Objectives
* Apply **VLANs** to isolate sensitive data.  
* Configure **static routes** on a router-on-a-stick setup.  
* Practice fundamental switch security (port security, MAC-sticky, BPDU-Guard).  
* Observe how segmentation slashes broadcast traffic and improves latency.  

## Repository Layout
```

.
├── Hospital Cisco Packet.pkt   # Packet Tracer simulation
└── README.md                   # You’re reading it

```

## Roadmap Ideas
* Add site-to-site or remote-access **VPNs** for off-site clinicians.  
* Integrate **cloud backups** for EMR/data redundancy.  
* Implement **802.1X NAC** for per-port authentication.  
* Replace static routes with **OSPF** once scale demands it.

## License
Released under the MIT License.


This version keeps things minimal—just the `.pkt` file and a standard README with no extra docs or acknowledgements, exactly as you requested. The feature list and learning goals mirror the high-level objectives of the original design .
