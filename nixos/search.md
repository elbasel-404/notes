linux_zen
magic sysrq
usbcore.autosuspend=-1

intel_idle.max_cstate=1: command not found
processor.max_cstate=1: command not found
acpi=noirq
acpi=strict
acpi_osi=Linux
pci=noacpi
acpi=off

boot.kernelParams = [
  "intel_idle.max_cstate=1"
  "processor.max_cstate=1"
  "pci=noacpi"
  "acpi=off"
];
boot.kernelParams = [ "kernel.sysrq=1" ];

