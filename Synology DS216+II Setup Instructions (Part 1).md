# Synology DS216+II Setup Instructions (Part 1)

This guide is written for **future you**, so you can set up your Synology DS216+II NAS without frustration. It includes all the steps you have done so far, including downloading necessary software, resetting the NAS, and reinstalling DiskStation Manager (DSM).

---

## Table of Contents
1. [What You Need](#what-you-need)
2. [Downloading Necessary Tools](#downloading-necessary-tools)
3. [Initial Setup](#initial-setup)
4. [Resetting the NAS](#resetting-the-nas)
5. [Reinstalling DSM](#reinstalling-dsm)
6. [Connecting to the NAS](#connecting-to-the-nas)
7. [Additional Notes](#additional-notes)
8. [Troubleshooting](#troubleshooting)

---

## What You Need

Before you start, make sure you have:
- **Synology DS216+II** unit.
- At least one hard drive (you are using: 1x 8TB and 1x 6TB).
- Power cable.
- Ethernet cable (to connect to your router).
- A computer on the same network (e.g., MacBookPro 14 M2 Max in your case).

---

## Downloading Necessary Tools

1. **Synology Assistant (Optional but Helpful):**
   - Visit the [Synology Download Center](https://www.synology.com/en-global/support/download).
   - Search for your model (**DS216+II**) in the search bar.
   - Under the **Desktop Utilities** section, download **Synology Assistant** for macOS.
   - Install and open Synology Assistant on your computer.

2. **User Manual:**
   - Go to the [Synology Support Page](https://www.synology.com/en-global/support/download).
   - Search for your model (**DS216+II**) and download the **Quick Installation Guide** or user manual.
   - Keep the manual handy for reference.

3. **Install Both:**
   - Install the Synology Assistant to help detect the NAS.
   - Refer to the manual for additional details on setup or troubleshooting.

---

## Initial Setup

1. **Install the Drives:**
   - Open the drive bays by removing the front panel.
   - Secure your drives in the trays and slide them back into the bays.
   - Ensure the drives click securely into place.

2. **Power On the NAS:**
   - Connect the NAS to your router using an Ethernet cable.
   - Plug in the power cable and press the **Power** button on the front panel.

3. **Wait for the NAS to Boot:**
   - Look for the **STATUS** LED to turn green, indicating the system is online.

4. **Discover the NAS:**
   - Open **Synology Assistant** or type `find.synology.com` in your browser to locate the NAS on your network.

---

## Resetting the NAS

If the NAS was partially set up before or you want to start fresh:
1. **Locate the RESET Button:**
   - The RESET button is on the **back panel**, near the LAN port. It is a small recessed button.

2. **Perform a Soft Reset (Network and Admin Settings Only):**
   - Use a paperclip to press and hold the RESET button.
   - Wait for the first beep (**approximately 4 seconds**) and release.

3. **Perform a Hard Reset (Complete Factory Reset):**
   - Use a paperclip to press and hold the RESET button.
   - Wait for the first beep (**approximately 4 seconds**) and release.
   - Then press and hold the RESET button again until you hear **three beeps**.
   - The NAS will return to a "Not Installed" state, wiping all settings.

4. **What Happens Next:**
   - The NAS will reset its network settings, admin credentials, and configuration.
   - After the hard reset, the system will require a fresh DSM installation.

---

## Reinstalling DSM

1. **Access the NAS After Reset:**
   - Open your browser and go to:
     - `find.synology.com` **or** `http://diskstation:5000`.
   - If that doesn’t work, use the IP address shown in Synology Assistant (e.g., `http://192.168.1.191`).

2. **Install DSM:**
   - Follow the on-screen instructions to install the latest DSM.
   - If prompted, format the drives (this will erase all data).
   - Set up your admin account with a secure username and password.

3. **Skip Synology Account Integration (Optional):**
   - If you don't want to use a Synology account, skip this step during setup.

---

## Connecting to the NAS

1. **Access DSM:**
   - Once DSM is installed, log in using the admin credentials you just created.
   - Use the IP address shown in Synology Assistant if needed.

2. **Set Up Your NAS:**
   - Configure storage, create volumes, and set up users as needed.
   - Install packages or services you need (e.g., file sharing, backups).

---

## Additional Notes

- **Why Reset?**
  - Resetting the NAS is useful if you've forgotten the admin credentials or want to start fresh.
- **Reset Button Details:**
  - Soft reset: Press and hold until **1 beep** (~4 seconds).
  - Hard reset: Press and hold until **1 beep** (~4 seconds), release, then press again until **3 beeps**.
- **Backup Before Reset:**
  - A hard reset erases all settings and data. Make sure to back up anything important beforehand.

---

## Troubleshooting

- **Can't Find the NAS?**
  - Ensure the NAS is connected to your router and powered on.
  - Double-check that the RESET process completed correctly.
  - Use the direct IP address (e.g., `http://192.168.1.191`) if `find.synology.com` doesn’t work.

- **Forgot Admin Credentials?**
  - Use the RESET button to perform a soft reset and regain access.

---

End of Guide.
