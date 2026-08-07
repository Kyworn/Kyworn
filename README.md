# Zorko / Kyworn

Technical Specialist at Apple by day, self-hosting and reverse engineering the rest of the time.
Linux, Proxmox, hardware, and LLMs.

I build these by orchestrating AI agents: the agents write the code, I own the architecture,
the integration, and the validation. Everything below runs.

## Infrastructure & tooling

**[ZorkoLab](https://github.com/Kyworn/ZorkoLab)** — my self-hosted infrastructure, documented
12 LXC containers on Proxmox VE · TrueNAS ZFS RAID1 · 17 services behind Nginx Proxy Manager and Cloudflare Zero Trust · local LLM inference on 2× Quadro P5000 · an autonomous agent that scans the stack weekly and reports its state

**[gnr-smu](https://github.com/Kyworn/gnr-smu)** — SMU telemetry map for AMD Granite Ridge (Ryzen 9800X3D)
457 undocumented floats, worked out by measurement and published with a per-field confidence level. CLI and PyQt6 GUI, a hardware gate that refuses to write on unvalidated configs, and an audit script that replays the docs against system sensors — its first run found 11 errors in my own notes.
[Telemetry map](https://github.com/Kyworn/gnr-smu/blob/master/PM_TABLE_MAP.md) · dumps from other Zen 5 parts very welcome

**[asus-debian-tools](https://github.com/Kyworn/asus-debian-tools)** — supergfxctl + asusctl on Debian 13
Install script plus the documentation that should come with it: prerequisites, step-by-step, symptom-by-symptom troubleshooting with the commands and logs to check, clean uninstall, and the known limits stated up front.

## Web

**[Wayvault](https://wayvault.net)** — World of Warcraft database & character planner
~116k cross-linked records (items, spells, quests, NPCs, instances, professions, achievements) with instant search, plus a planner that auto-gears a full character including enchants and gems. Live and maintained.

## Research

**[PentaNet](https://github.com/Kyworn/PentaNet-v1.0)** — native pentanary {-2,-1,0,+1,+2} quantization for LLMs
−6.4% PPL vs ternary BitNet at 124M params · 3 seeds · WikiText-103. The advantage does not survive to 345M, and the scaling investigation says why.
[Paper](https://github.com/Kyworn/PentaNet-v1.0/blob/main/paper/PentaNet_Technical_Report.pdf) · [Model](https://huggingface.co/Kyworn/pentanet-124m)

**[ShiftQuant](https://github.com/Kyworn/ShiftQuant)** — limits of shift-based post-training quantization
No 7-value grid escapes the coverage/gap tradeoff · AWQ recovers 22% at isocompression · grid and AWQ gains are 93.6% orthogonal. The EDC search is written up as a negative result.
[Paper](https://github.com/Kyworn/ShiftQuant/blob/main/paper/shiftquant.pdf)

## Also

Lyon Transit Viewer (real-time TCL network, React / Mapbox / SpacetimeDB) · Hub'Eau (tap water quality by commune, React / FastAPI) · HID Nintendo LED (published on the Arch AUR) · Seerr Webhook · ZorkoPower · TapTracker · Thermal-Dash

## Stack

Proxmox · LXC · Docker · TrueNAS/ZFS · Cloudflare Zero Trust · Nginx · Python · Shell · TypeScript · React · PyTorch · Ghidra
