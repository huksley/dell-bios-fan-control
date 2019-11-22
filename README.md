## dell-bios-fan-control

#### A user space utility to set control of fans by bios on Dell XPS 13 9380 Laptops.

Allows to control the fans by bios or i8kctl utils.

  

### Usage

To enable SMBIOS control:

<pre>
dell-bios-fan-control 1
</pre>

To disable SMBIOS control:

<pre>
dell-bios-fan-control 0
</pre>

After disabling SMBIOS control of fans you can set fan speed by i8kctl:

<pre>
i8kctl fan 1 1
</pre>

  

### Caveats

* The BIOS of some newer Dell laptops (9560, ...)
  will override the speed you set unless you disable the BIOS control.

* This tool allows to enable or disable bios control of fans to
  use i8kmon instead

* Sometimes disables brightness control and power button to suspend 

### Credits

* All credits belong to: https://github.com/clopez/dellfan
* https://www.dell.com/community/Linux-Developer-Systems/XPS-13-9350-fan-control/m-p/5036618/highlight/true#M6457
