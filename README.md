# 🐧 Project: Mastering the Linux Environment

## Introduction

This project series will introduce you to the **Linux kernel** and its application in **server environments**. Linux is the core of countless operating systems, powering everything from your phone to major data centers. We will be using **Debian**, a stable and popular Linux distribution, to build a strong foundation in server administration.

By understanding the environment beneath your programs and the services behind the Cloud, you will become a more capable programmer and gain valuable skills for controlling machines and servers.

> "But this wasn't to be just any penguin. Above all, Linus wanted one that looked happy, as if it had just polished off a pitcher of beer and then had the best sex of its life."
> — *Just for Fun: The Story of an Accidental Revolutionary* (Linus Torvalds, David Diamond)

---

## 💻 Virtualization

To ensure a standardized and risk-free practice environment, we will use **virtualization**.

**Virtualization** allows you to run **Virtual Machines (VMs)**—virtual computers—on your existing operating system (the **Host**). This means you can run Linux, Windows, or macOS simultaneously in separate windows.

* **Requirement:** Install the hypervisor **VirtualBox**.

---

## ⚙️ Installation: Setting up the Debian VM

You will install the Debian operating system inside a Virtual Machine. Operating systems are typically installed using a "disk image" (an **ISO file**).

* **Recommended Disk Image:** Debian **"netinst" ISO installer**.

### Installation Steps:

1.  **Create the VM:** Use VirtualBox to create a new Virtual Machine instance, allocating resources like RAM and storage.
2.  **Start the VM and Attach the ISO:**
    * Start the newly created VM.
    * Attach the Debian ISO file as an optical drive (like inserting a CD/DVD).
3.  **Follow the Installer:** Proceed through the Debian installer steps.
4.  **Reboot:** Once the installation is complete, the VM will reboot into a ready-to-use Debian system.

### 🛑 Graceful Shutdown

Always shut down your VM properly to prevent data corruption.

* **Recommended Method:** Use **"ACPI Shutdown"** from the VirtualBox menu (or the equivalent host-key combination). This simulates pressing the power button on a real computer.

---

## ✅ Functional Requirements (Assessment)

The following points will be assessed to confirm the successful setup of the Linux environment.

| # | Task | Assessment Question | Success Criteria |
| :--- | :--- | :--- | :--- |
| **1** | **Hypervisor Setup** | Is the virtualization software (VirtualBox) correctly installed on the machine? | The auditee can successfully start the virtualization software. |
| **2** | **VM Availability** | Is a Virtual Machine with a version of Debian already installed available? | The auditee can display the installed Debian VM. |
| **3** | **System Boot** | Does the virtual machine boot Debian properly? | The Debian system boots completely (displays the login prompt) in less than 2 minutes. |
| **4** | **System Control** | Could the auditee log in and shut down the VM using a command line? | The auditee successfully logs into the console and executes the proper command (e.g., `shutdown now` or `poweroff`). |