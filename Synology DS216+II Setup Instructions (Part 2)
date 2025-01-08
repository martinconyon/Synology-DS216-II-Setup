# Synology DS216+II Setup Instructions (Part 2)

This guide picks up where the first guide left off and helps you configure storage, understand RAID types, and start using your NAS for transferring files. It continues to be a **cookbook guide for future you**.

---

## Table of Contents
1. [Understanding Storage Pools and RAID Types](#understanding-storage-pools-and-raid-types)
2. [Configuring Storage](#configuring-storage)
3. [Creating Shared Folders](#creating-shared-folders)
4. [Transferring Files to Your NAS](#transferring-files-to-your-nas)
5. [Best Practices](#best-practices)

---

## Understanding Storage Pools and RAID Types

### **1. Storage Pools**
- A **Storage Pool** is a grouping of physical drives that act as a single logical unit.
- It allows you to configure RAID types for redundancy and organize storage volumes.

### **2. RAID Types**
The common RAID types available on a Synology NAS:

- **Synology Hybrid RAID (SHR):**
  - Default RAID type for Synology.
  - Offers flexibility with mixed drive sizes.
  - Provides redundancy (e.g., 1-drive fault tolerance).

- **RAID 1:**
  - Mirrors data across two drives.
  - Provides redundancy but requires drives of equal size.

- **Basic:**
  - No redundancy; each disk is used independently.
  - If a drive fails, data is lost.

- **Other RAID Types:** Advanced options like RAID 5/6 are available for systems with more drives.

**Recommendation:** For most use cases, SHR is the best balance between flexibility and data protection.

---

## Configuring Storage

### **Step 1: Open Storage Manager**
1. From the DSM interface, click **Storage Manager** (available in the Main Menu or sidebar).

### **Step 2: Check Existing Configuration**
1. Navigate to **Storage Pool 1**.
   - Confirm the RAID type (likely SHR).
   - Verify that both drives are listed as healthy.

2. If the Storage Pool is not set up:
   - Follow the on-screen wizard to create a new Storage Pool.
   - Choose the RAID type (SHR recommended).
   - Format the drives (this will erase any existing data).

### **Step 3: Create a Volume**
1. Go to the **Volume** tab in Storage Manager.
2. Click **Create** and select the existing Storage Pool.
3. Choose a file system:
   - **Btrfs:** Recommended for snapshots and advanced data protection.
   - **EXT4:** Simpler and slightly faster.
4. Complete the wizard to initialize the volume.

---

## Creating Shared Folders

Shared folders allow you to organize and store files on your NAS.

### **Step 1: Open Control Panel**
1. Go to **Control Panel > Shared Folder**.
2. Click **Create** to make a new shared folder.

### **Step 2: Configure the Folder**
1. Enter a name for the folder (e.g., `Documents`, `Photos`, `Backups`).
2. Choose the volume where it will be stored (e.g., Volume 1).
3. Set permissions:
   - **Admin Account:** Full access.
   - Other users (if created): Assign access as needed.

### **Step 3: Advanced Options**
- Enable encryption (optional) for sensitive folders.
- Enable data integrity protection if using Btrfs.

---

## Transferring Files to Your NAS

### **Option 1: Direct USB Transfer**
1. Plug an external USB drive into one of the NAS USB ports.
2. Open **File Station** in DSM.
   - You’ll see the USB drive listed under "External Devices."
3. Drag and drop files from the USB drive to your shared folders.

### **Option 2: Network Transfer**
1. On your computer:
   - **macOS:** Open Finder, press `Command + K`, and type `smb://[NAS_IP]` (e.g., `smb://192.168.1.191`).
   - **Windows:** Open File Explorer and type `\\[NAS_IP]` in the address bar.
2. Log in with your NAS admin account.
3. Drag and drop files into the shared folders.

### **Option 3: Synology Drive (Optional)**
1. Install **Synology Drive Server** from the Package Center.
2. Install **Synology Drive Client** on your computer.
3. Set up a sync task between your computer and the NAS for continuous synchronization.

---

## Best Practices

1. **Data Scrubbing:**
   - Schedule regular data scrubbing (every 1-3 months) in Storage Manager to ensure data integrity.

2. **Backups:**
   - Use **Hyper Backup** to back up critical data to an external USB drive or another NAS.
   - Keep a secondary backup off-site if possible.

3. **User Permissions:**
   - Limit user access to sensitive folders for better security.

4. **Monitor System Health:**
   - Regularly check Storage Manager for disk health and system status.

---

Your NAS is now fully configured and ready to use for file storage and sharing. Let me know if you need help with anything else!
