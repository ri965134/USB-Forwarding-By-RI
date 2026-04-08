# USB Forwarding By RI - USB over IP Windows GUI Client

A lightweight, powerful **Windows Graphical User Interface (GUI)** designed to manage and forward USB devices over a TCP/IP network. Built on top of the robust **USB/IP protocol**, this tool allows you to seamlessly share and connect remote USB hardware to your Windows PC as if it were physically plugged into your local machine.

Whether you are forwarding Android devices for development, sharing storage drives over a LAN, or remotely accessing biometric scanners for CSP operations, **USB Forwarding By RI** completely automates the complex backend networking and driver installations.

## 🚀 Key Features & Capabilities

* **Automated USB/IP Driver Setup:** Silently installs the required Windows Kernel-level drivers (`usbip_vhci_ude.inf`), root security certificates, and virtual USB hub hardware on the very first run.
* **Smart Network Scanner:** Automatically pings your target IP address and retrieves a clean, readable list of all exportable USB devices currently attached to the remote host.
* **Multi-Device Virtualization:** Select, attach, and detach multiple USB devices simultaneously. The app intelligently tracks independent Virtual Windows Ports (0-15) for conflict-free management.
* **Pre-Flight Network Diagnostics:** Built-in latency and routing checks ensure the host IP is reachable before attempting a connection, providing human-readable troubleshooting steps if the network fails.
* **Dynamic Theme Engine:** A responsive, data-grid UI that automatically adapts to your system's Windows 10/11 Light or Dark mode registry settings.

## 🎯 Common Use Cases

* **Android USB Forwarding:** Access Android phones connected to remote servers for ADB debugging or file transfers.
* **Remote Biometric Scanners:** Ideal for network operators and Customer Service Points (CSP) needing to share fingerprint or iris scanners over a local network.
* **Wireless Hardware Access:** Share printers, webcams, or flash drives across your home or office Wi-Fi without moving cables.

## ⚙️ Installation & Usage Guide

**Important:** For the automated installer to work, `USB Forwarding By RI.exe`, `usbip.exe`, and the `Driver` folder must remain together in the exact same directory.

1. **Run the Executable:** Double-click `USB Forwarding By RI.exe`. The software will request Administrator privileges once to silently install the virtual hardware and place a standard shortcut on your desktop.
2. **Launch the App:** Open the program using the newly created desktop shortcut.
3. **Connect to Host:** Enter the **Target IP Address** (e.g., your phone or server IP) and the TCP Port (default: 3240).
4. **Scan & Attach:** Click **Scan Network** to discover connected USB devices. Tick the checkboxes next to the desired hardware and click **Attach Selected**.

## 🛠️ Troubleshooting & Driver Issues

If devices fail to attach or the connection is actively refused, verify that the virtual USB driver was successfully initialized by Windows:

1. Open Windows **Device Manager**.
2. Scroll down and expand the **Universal Serial Bus controllers** section.
3. Look for the **`usbip-win VHCI(ude)`** driver.
4. **Fix:** If this driver is missing or showing an error triangle, delete your desktop shortcut and run the main `.exe` file from your downloaded folder again to force a clean reinstallation.

## 🤝 Support & Contact

**Developed by:** Rahil Islam  
**Technical Support:** RI965134@GMAIL.COM  

If you encounter bugs, need help with network configurations, or want to suggest new features, please reach out via email or open an Issue in this GitHub repository.
