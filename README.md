\# Network Packet Capture



A practical packet capture/sniffer project focused on learning real traffic analysis and building a reusable capture pipeline.



\## What it does

\- Captures packets from a selected network interface

\- Decodes basic L2/L3/L4 headers (Ethernet/IP/TCP/UDP/ICMP)

\- Prints structured output to console (later: JSON + file output)

\- Supports filtering (later: BPF-like filters / protocol filters)



\## Tech / Approach

This repo includes `jpcap/` (Java packet capture library sources). The main capture app can be built on top of it.



\## Requirements

\### Windows

\- Install \*\*Npcap\*\* (recommended) in WinPcap-compatible mode.

\- Run terminal as Administrator (capture needs elevated permissions).



\### Linux (Kali/Ubuntu)

\- Install libpcap dev tools:

&nbsp; - Debian/Kali: `sudo apt install libpcap-dev`

\- Run with sudo (or set capabilities later).



\## Repo Structure

\- `jpcap/` — embedded library source (tracked normally, NOT a submodule)

\- `src/` — (create this) your capture application code

\- `captures/` — (ignored) packet capture outputs



\## Quick Start (Planned)

> You will add these commands once the app entrypoint exists.



\### Build

\- `./build.sh` (Linux)

\- `build.ps1` (Windows)



\### Run

\- `sudo ./run.sh` or `.\\run.ps1`



\## Output Format (Example)

