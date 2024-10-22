

**Key Components of Computer Hardware:**

* **CPU (Central Processing Unit):**
    * Often referred to as the "brain" of the computer.
    * Executes program instructions, performs arithmetic and logical operations, and manages data flow within the computer.
* **RAM (Random Access Memory):**
    * A type of volatile memory that temporarily stores data and program instructions needed by the CPU.
    * Provides fast read and write access to data and affects overall system speed and performance.
* **Firmware:**
    * Specialized software programmed into hardware components that provides low-level control.
    * Manages hardware functions like the booting process and controls hardware without a full operating system.
    * Found in embedded systems and device firmware updates.
* **Mass Storage:**
    * Devices used to store data permanently, even when the computer is turned off.
    * Examples include HDDs, SSDs, and optical discs.
    * Retains operating systems, applications, and user data.
    * Typically slower than RAM but offers much larger capacity.

**Additional Components:**

* **Motherboard:** Connects all hardware components and allows communication between them.
* **PSU (Power Supply Unit):** Converts electrical power from an outlet into usable power for the computer's internal components.
* **GPU (Graphics Processing Unit):** Specialized hardware for rendering images, video, and animations.
* **NIC (Network Interface Card):** Allows the computer to connect to networks and communicate with other devices.

**Understanding CPU, RAM, Firmware, and Mass Storage in Linux:**

* **CPU:**
    * Use `lscpu` to get detailed information about the CPU architecture and its capabilities.
    * Use `uname` to obtain kernel information, including the kernel version and architecture.
* **RAM:**
    * Use `cat /proc/meminfo` to view detailed information about the system's memory usage.
    * Use `free` to get a quick overview of the total, used, and free memory (both RAM and swap).
* **Firmware:**
    * Understand the roles of BIOS and UEFI in system startup and initialization.
    * BIOS is the traditional firmware interface, while UEFI is the modern standard with enhanced features.
* **Mass Storage:**
    * Use `df -h` to report the disk space usage of file systems.
    * Understand storage interface technologies like SCSI, IDE, SATA, and USB.

**Hardware Resources and Connectivity:**

* **Hardware Resources:**
    * I/O Ports, I/O Memory, Interrupt Requests (IRQ), Direct Memory Access (DMA).
* **Viewing Hardware:**
    * Use `lsusb` to list USB devices.
    * Use `lspci` to list PCI devices.
* **Hardware Connectivity:**
    * Internal and external buses.
    * PCI standards, bridges, and channels.
    * Northbridge and Southbridge architecture.

**Hardware Subsystem Tools:**

* **udev:** Device manager for Linux.
* **sysfs:** Virtual filesystem for kernel objects.
* **procfs:** Virtual filesystem for process and system information.
* **HALD (Hardware Abstraction Layer Daemon):** Replaced by udev and D-Bus.
* **D-Bus:** Inter-process communication system.

**Kernel Modules:**

* Extend the kernel's functionality without modifying the kernel source code.
* Load and unload modules using `modprobe` and `rmmod`.
* View loaded modules using `lsmod`.
* Use `modinfo` to get detailed information about a specific module.

