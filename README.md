# 🍏 Apple FireWire iSight on Windows

Make your **Apple iSight FireWire** webcam fully functional on modern versions of **Windows (XP → 11)** using legacy **Unibrain ubCore** and **CMU 1394 Digital Camera** drivers.

---

## 📸 About

Apple’s **iSight FireWire camera** (released in 2003) still provides surprisingly good image quality — but under Windows it often appears **overexposed** or **too bright**, especially when using the default **Microsoft 1394 Legacy driver**.

This repository collects all known working **FireWire (IEEE 1394) drivers and tools** that help bring the iSight camera back to life on Windows.  
It also includes documentation and tested configurations that fix the exposure issue.

---

## 📦 Contents

The archive contains all official and historical releases from two key sources:

### 🧩 Unibrain Drivers (ubCore / Fire-i / FireAPI)

From [Unibrain’s official site](https://www.unibrain.com/downloads/):

- **ubCore™ 6.00 Pro (x86/x64)** – FireWire 800 drivers (Vista/7/8/10)
- **ubCore™ 6.00 (x86/x64)** – For end-users (webcams & storage)
- **ubCore™ 5.80 Pro (x64)** – Legacy version (Windows Vista–10)
- **Fire-i™ 4.0** – Drivers & camera control application
- **FireAPI™ 6.00 (Eval)** – 1394a/b development toolkit
- **Fire-i API™ 4.0 (Eval)** – IIDC FireWire camera SDK
- **Fire-i X™ 2.6 (Full)** – ActiveX / .NET control SDK

---

### 🧠 CMU 1394 Digital Camera Driver (Carnegie Mellon University)

From [CMU Robotics Institute](https://www.cs.cmu.edu/~iwan/1394/downloads/index.html):

Versions included:
- `6.4.6 (signed)` – September 26, 2011  
- `6.4.6 (unsigned)` – August 6, 2011  
- `6.4.6 beta` – March 13, 2011  
- `6.4.5` → `4.1` (2000–2008) – Full version history with source code

Each release contains:
- 📁 `1394cameraXXX.exe` — Driver installer  
- 💾 `*_src.zip` — Original source code archives

---

## ⚙️ Installation & Usage

1. **Install the CMU 1394 Camera Driver**  
   Use the latest signed version (`1394camera646.exe`).  
   After installation, your iSight should appear in the **1394 Camera Demo** app.

2. **Check Image Quality**  
   The overexposure issue should be gone. You’ll notice a natural color balance and proper contrast.

3. **Use with Other Apps (OBS, Telegram, Zoom, etc.)**  
   Since the CMU driver doesn’t register as a native DirectShow camera, you can:
   - Open **1394 Camera Demo**  
   - Capture its window in **OBS Studio**  
   - Start **Virtual Camera** in OBS  
   - Select "OBS Virtual Camera" in Telegram / WhatsApp / Zoom

✅ This effectively makes the iSight usable as a webcam on Windows again — even in 2025.

---

## 🖼️ Comparison (Before / After)

| Microsoft 1394 Legacy Driver | CMU 1394 Camera Driver |
|------------------------------|------------------------|
| Overexposed, washed-out image | Correct exposure, natural colors |

*(Screenshots available in `/screenshots` folder)*

---

## 💾 Compatibility

| Windows Version | Status |
|------------------|--------|
| XP / Vista / 7 | ✅ Supported |
| 8 / 8.1 / 10 | ✅ Tested, working |
| 11 | ⚠️ Not fully tested (driver signing may require disabling Secure Boot) |

---

## 📚 References

- [Using Firewire Apple iSight on Windows Vista/7](https://greenteapanda.wordpress.com/2009/02/12/using-firewire-apple-isight-on-windows-vista7/)
- [Unibrain Official Downloads](https://www.unibrain.com/downloads/)
- [CMU 1394 Camera Driver Project](https://www.cs.cmu.edu/~iwan/1394/downloads/index.html)
- [Apple iSight FireWire Specs (EveryMac)](https://everymac.com/systems/by_capability/isight_specs.html)

---

## 🧰 Archive Info

All installers and source files are provided **as-is**, for archival and educational purposes.  
Please respect original licenses and copyrights.

---

## 🪄 Credits

- **Unibrain Ltd.** – ubCore, Fire-i, FireAPI drivers  
- **Christopher R. Baker (CMU)** – CMU 1394 Digital Camera Driver  
- **John Weekend** – Testing, documentation, OBS virtual camera workaround

---

## 🪐 License

This repository itself (readme and archive organization) is released under the **MIT License**.  
Individual driver packages retain their **original licenses**.

---

> 🧡 2003 hardware, 2025 usability.  
> Thanks to community persistence, the Apple iSight FireWire camera lives on.
