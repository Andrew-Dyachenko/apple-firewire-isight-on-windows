# 🍏 Apple FireWire iSight on Windows

Make your **Apple iSight FireWire** webcam fully functional on modern versions of **Windows** using legacy **Unibrain ubCore** and **CMU 1394 Digital Camera** drivers — archived and preserved for the future.

---

## 📸 About

Apple’s **iSight FireWire camera** (2003) can still deliver excellent image quality — but under Windows it often appears **overexposed** when using the standard **Microsoft 1394 Legacy driver**.

This repository collects and preserves **all known working FireWire (IEEE 1394) drivers and tools** that can help restore proper image quality and functionality of the Apple iSight camera on Windows systems.

🧭 This is an **archival repository** — created to ensure these legacy drivers remain available even if the original download sources disappear.

---

## 📦 Contents

The archive includes all official and historical releases from two primary sources:

### 🧩 Unibrain Drivers (ubCore / Fire-i / FireAPI)

From [Unibrain’s official site](https://www.unibrain.com/downloads/):

- **ubCore™ 6.00 Pro (x86/x64)** – FireWire 800 drivers (Vista/7/8/10)
- **ubCore™ 6.00 (x86/x64)** – For end-users (webcams & storage)
- **ubCore™ 5.80 Pro (x64)** – Legacy version (Vista–10)
- **Fire-i™ 4.0** – Drivers & camera control application
- **FireAPI™ 6.00 (Eval)** – 1394a/b development toolkit
- **Fire-i API™ 4.0 (Eval)** – IIDC FireWire camera SDK
- **Fire-i X™ 2.6 (Full)** – ActiveX / .NET control SDK

⚠️ **Note:** Unibrain’s ubCore drivers are **unstable on Windows 10+**, frequently causing system crashes (BSOD).  
However, they may work more reliably on **older Windows versions (XP–7)** and have historically been used to fix iSight’s exposure issue on those systems.

---

### 🧠 CMU 1394 Digital Camera Driver (Carnegie Mellon University)

From [CMU Robotics Institute](https://www.cs.cmu.edu/~iwan/1394/downloads/index.html):

Versions included:
- `6.4.6 (signed)` – September 26, 2011  
- `6.4.6 (unsigned)` – August 6, 2011  
- `6.4.6 beta` – March 13, 2011  
- `6.4.5` → `4.1` (2000–2008) – Full version history with source code

Each release includes:
- 📁 `1394cameraXXX.exe` — Driver installer  
- 💾 `*_src.zip` — Original source code archives

---

## ⚙️ Installation & Usage

1. **Install the CMU 1394 Camera Driver**  
   Use the latest signed version (`1394camera646.exe`).  
   After installation, your iSight should appear in the **1394 Camera Demo** app.

2. **Check Image Quality**  
   The overexposure issue should disappear — the image becomes properly exposed with natural contrast.

3. **Use with Other Apps (OBS, Telegram, Zoom, etc.)**  
   The CMU driver doesn’t register a native DirectShow camera.  
   You can work around this easily:
   - Open **1394 Camera Demo**
   - Capture its window in **OBS Studio**
   - Start **OBS Virtual Camera**
   - Select “OBS Virtual Camera” in Telegram / WhatsApp / Zoom

✅ This setup makes the iSight FireWire camera usable again in 2025 — even on Windows 10.

---

## 🖼️ Image Comparison

| Microsoft 1394 Legacy Driver | CMU 1394 Camera Driver |
|------------------------------|------------------------|
| Overexposed, high contrast | Balanced, natural colors |

*(See `/screenshots` folder for actual results.)*

---

## 💾 Compatibility

| Windows Version | Status |
|------------------|--------|
| XP / Vista / 7 | 🟡 Likely compatible (per original driver documentation) |
| 8 / 8.1 / 10 | 🟢 Personally tested on Windows 10 x64 — fully functional |
| 11 | ⚠️ Untested (driver signing issues may require disabling Secure Boot) |

> 📋 The drivers were designed for Windows XP–10 according to official documentation.  
> This repository’s maintainer has **only tested on Windows 10 x64**.

---

## 📚 References

- [Using Firewire Apple iSight on Windows Vista/7](https://greenteapanda.wordpress.com/2009/02/12/using-firewire-apple-isight-on-windows-vista7/)
- [Unibrain Official Downloads](https://www.unibrain.com/downloads/)
- [CMU 1394 Camera Driver Project](https://www.cs.cmu.edu/~iwan/1394/downloads/index.html)
- [Apple iSight FireWire Specs (EveryMac)](https://everymac.com/systems/by_capability/isight_specs.html)

---

## 🧰 Archive Info

This repository is **archival** — intended to preserve all related drivers, SDKs, and documentation for future users and enthusiasts of the Apple iSight FireWire camera.

All files are provided **as-is** for educational and historical purposes.  
Please respect the original authors’ licenses and copyrights.

---

## 🪄 Credits

- **Unibrain Ltd.** – ubCore, Fire-i, FireAPI drivers  
- **Christopher R. Baker (CMU)** – CMU 1394 Digital Camera Driver  
- **John Weekend** – Testing, documentation, and OBS virtual camera workaround

---

## 🪐 License

The repository itself (README and organization) is distributed under the **MIT License**.  
Individual driver packages remain under their **original licenses**.

---

> 🧡 2003 hardware, 2025 usability.  
> Thanks to community persistence, the Apple iSight FireWire camera still shines today.
