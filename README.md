# Apple FireWire iSight on Windows

![Tested: Windows 10 x64](https://img.shields.io/badge/Tested-Windows%2010%20x64-blue)
![Archive project](https://img.shields.io/badge/Archive-Project-lightgrey)
![Status: Experimental](https://img.shields.io/badge/Status-Experimental-yellow)

This repository preserves all known working (and partially working) FireWire (IEEE 1394) drivers for Windows —  
collected from **Unibrain** and **Carnegie Mellon University (CMU)** websites.  
It exists as an **archival project** to ensure that Apple FireWire iSight and other IEEE 1394 cameras  
remain usable even if the original sources someday disappear.

📦 Repository: [https://github.com/Andrew-Dyachenko/apple-firewire-isight-on-windows](https://github.com/Andrew-Dyachenko/apple-firewire-isight-on-windows)

---

## 💡 Purpose

This project was created primarily for enthusiasts who still use the legendary **Apple iSight FireWire camera (2003)**  
on modern Windows systems.  

All drivers are stored here **as-is**, unmodified and unaltered, exactly as they were distributed by their authors.  
I did not modify, recompile, or patch any of the files — only gathered them for long-term preservation.

---

## 🧩 Included Drivers

### From **Unibrain**
Source: [https://www.unibrain.com/downloads/](https://www.unibrain.com/downloads/)

- ubCore™ 6.00 (32-bit / 64-bit)
- ubCore™ 6.00 Pro (32-bit / 64-bit)
- ubCore™ 5.8 Pro (64-bit)
- FireAPI™, Fire-i API™, Fire-i X™ SDKs (evaluation versions)
- Fire-i™ 4.0 drivers & control application (32-bit / 64-bit)

⚠️ **Note:** Unibrain ubCore drivers may cause system instability (BSOD)  
**only when used with Apple FireWire iSight camera on Windows 10 x64**.  
They should work properly on older Windows versions such as XP, Vista, 7, and 8.  
This does **not** mean Unibrain’s software is faulty — the issue is specific to this combination of hardware and OS.

---

### From **Carnegie Mellon University (CMU)**
Source: [https://www.cs.cmu.edu/~iwan/1394/downloads/index.html](https://www.cs.cmu.edu/~iwan/1394/downloads/index.html)

- CMU 1394 Digital Camera Driver versions **4.1 → 6.4.6** (including signed, unsigned, and beta builds)
- Installation utilities and source code archives

---

## 🧠 Compatibility

These drivers were **tested by me personally on Windows 10 64-bit**.  
Earlier Windows versions (XP, Vista, 7, 8) are officially listed as supported by Unibrain and CMU,  
so they should also be compatible in theory — but I have not tested them myself.

---

## 🧰 Practical usage notes

For the **CMU 1394 driver (6.4.6 signed)**, the Apple iSight FireWire camera produces a correct image  
with balanced brightness and contrast.  

If you use the **Microsoft 1394 Legacy driver**, the image may appear overexposed,  
though it works in more applications (OBS, Telegram, etc.).  

To use the CMU driver effectively:
- Open the `1394Camera Demo` application that comes with it  
- Capture its window via **OBS Studio**
- Enable **OBS Virtual Camera**
- Select it in **Telegram**, **WhatsApp Desktop**, **Zoom**, or any other video chat app.

It’s not the most convenient setup, but it’s a small price to pay for bringing a 2003 FireWire camera back to life in 2025!

---

## 📸 Before / After Example

*(Screenshots showing overexposed vs corrected image can be placed here later)*

---

## 🧾 License notice

All drivers remain under their **original authors’ licenses** —  
Unibrain and Carnegie Mellon University retain all rights to their respective software.

This repository itself (the collection and documentation) is provided under the  
**MIT License**, purely for archival and educational purposes.

---

## 🤝 Community

If you manage to improve stability, find newer driver versions, or successfully test  
on other Windows releases — contributions and reports are welcome.  
Please open an issue or pull request on GitHub.

---

**Maintained by:** [Andrew Dyachenko](https://github.com/Andrew-Dyachenko)  
**Purpose:** Long-term preservation of legacy FireWire camera drivers  
**Created:** 2025  
