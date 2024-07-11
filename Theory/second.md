1. The Linux system initializes sequence from power on to when the user interface is ready.
2. BIOS (Basic Input/Output System) :- 
   a) This is the first stage in the Booting process.
   b) Initializes the POST(Power on self test) process, where the system hardware, including the screen and keyboard, and 
      the main memory are tested.
   c) The BIOS software stored on a ROM chip on the motherboard.
   d) After this stage the rest of the Boot process is controlled by operating system.
3. MBR (Master Boot Record) and Boot Loader.
   a) The system control passes from the BIOS to boot loader.
   b) Boot Loader can be found in system Hard disk either in boot sector (BIOS/MBR systems) or the EFI partition
      (UFEI Unified Extensible Firmware Interface or EFI/UEFI systems).
   c) The boot loader loads the kernel image and the initial RAM disk or filesystem into memory.
      eg:- boot loaders are GRUB (Grand Unified Boot Loader), ISOLINUX (from booting from removable media),
           and DAS U-Boot (for booting on embedded devices/appliances)

4. The boot loader has two stages :-
   i) The boot loader resides in the MBR.
      - The first stage boot loader finds the partition table and finds a bootable partition from that table.
   ii) The second boot loader resides under /boot.
      - The second boot loader finds and loads the GRUB into RAM 
      - It is responsible for displaying a splash on screen for user to choose os to boot 
      - The boot loader loads the kernel of the selected OS into RAM and passes control to the kernel.