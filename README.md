
---

## 🛡️ **Repo Name:** `obsidian-command-chain`

---

## 📁 **Directory Structure**
```
obsidian-command-chain/
├── OCC.sh                     # The master script (fully consolidated)
├── vanish/
│   ├── vanisher_of_obsidian.ps1   # Windows cleanup
│   └── vanisher_of_obsidian.sh    # Linux cleanup
├── ops/                      # Optional: Where operation logs will be stored
├── README.md
├── LICENSE
└── .gitignore
```

---

## 📜 **README.md**
```markdown
# 🛡️ Obsidian Command Chain (OCC)

**Penetrate. Execute. Vanish. Debrief.**  
A fully modular red-team penetration testing framework designed to operate with stealth, precision, and power. Built by a warrior, for warriors.

---

## 🔥 What It Does

The OCC executes the full lifecycle of a red-team operation:
1. **Obsidian Drone** – Stealth recon and enumeration
2. **Spear of Obsidian** – Targeted, low-noise exploitation
3. **Vanisher of Obsidian** – OS-aware cleanup module (Windows/Linux)
4. **Obsidian Debrief** – Automatically generates a professional After-Action Report (Markdown format)

---

## 💻 Usage

```bash
chmod +x OCC.sh
./OCC.sh
```

The OCC will guide you step-by-step:
- Ask for the target
- Choose stealth or aggressive mode
- Run recon, exploitation, OS-aware cleanup prep
- Generate a red-team-style AAR

---

## 📁 Output Example

```
ops/OP-OBSIDIAN-20250413-xxxx/
├── recon/
├── recon/exploits/
├── vanish/
│   └── vanisher.ps1 / vanisher.sh
└── debrief/
    └── AAR_OP-OBSIDIAN-20250413-xxxx.md
```

---

## ⚔️ Requirements

- `nmap`, `whatweb`, `curl`, `sshpass`, `smbclient`, `nikto`, `searchsploit`, `nuclei`, `rustscan`
- Optional: `wappalyzer`, `hydra`

---

## ⚠️ Legal Disclaimer

This tool is for **authorized use only**. Do not use against targets without proper permissions. You are responsible for your actions.

---

## 🧠 Inspired By

- The B-52 Framework Model: *Penetrate – Execute – Vanish*
- Red-team tradecraft
- War room-style planning
- Obsidian Vault workflows
```

---

## 📦 GitHub Initialization Instructions (local)

```bash
mkdir obsidian-command-chain && cd obsidian-command-chain
touch OCC.sh && chmod +x OCC.sh
mkdir vanish ops
# Add your vanisher_of_obsidian.ps1 and .sh files into the vanish folder
git init
echo "# Obsidian Command Chain" > README.md
echo "ops/" > .gitignore
touch LICENSE  # I recommend MIT License
git add .
git commit -m "Initial commit: OCC framework with recon, execution, cleanup, debrief"
gh repo create obsidian-command-chain --public --source=. --remote=origin --push
```
