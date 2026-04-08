# USB Forwarding By RI

A lightweight, powerful Windows graphical client to forward and manage USB devices over a network (TCP/IP). Built to work seamlessly with the USB/IP protocol, this tool allows you to connect remote USB devices (like biometric scanners, mobile devices, or storage drives) to your PC as if they were physically plugged in.

## ✨ Features
* **Automated Setup:** Silently installs required Kernel-level drivers, root certificates, and virtual USB hub hardware on the first run.
* **Network Scanner:** Instantly ping and scan a target IP address to list all available exportable USB devices.
* **Multi-Device Management:** Attach and detach multiple USB devices simultaneously with precise Virtual Port tracking.
* **Smart Diagnostics:** Built-in network health checks and human-readable error handling.
* **Dynamic UI:** Clean, responsive DataGrid interface that automatically adapts to Windows Light/Dark mode.

## 🚀 Installation & Usage

**Important:** Ensure that `USB Forwarding By RI.exe`, `usbip.exe`, and the `Driver` folder are all kept together in the same directory.

1. Double-click **`USB Forwarding By RI.exe`** to initiate the setup. The software will automatically install the necessary drivers and create a desktop shortcut.
2. Launch the application from the new desktop shortcut.
3. Enter the **Phone IP** (or host server IP) and the Port (default is 3240).
4. Click **Scan Network** to discover available USB devices.
5. Check the box next to the desired device(s) and click **Attach Selected**.

## 🛠️ Troubleshooting

If you experience connection problems or the devices fail to attach, verify that the virtual USB driver was installed correctly by Windows:

1. Open Windows **Device Manager**.
2. Scroll down and expand the **Universal Serial Bus controllers** section.
3. Look for the **`usbip-win VHCI(ude)`** driver.
4. **If the driver is missing:** Delete the desktop shortcut and run `USB Forwarding By RI.exe` from your main folder again to force a clean reinstallation.

## 📞 Contact & Support

**Developer:** Rahil Islam  
**Email:** RI965134@GMAIL.COM  

For bug reports, technical help, or feature requests, please reach out via email or open an issue in this repository.
