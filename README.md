In theory:
Intel ACPI contains MPS v1.4 Tables, and MPS v1.4 contains APIC.

ACPI (MPS v1.4 (APIC))

ACPI [MPS v1.4 [APIC]]

https://en.wikipedia.org/wiki/MultiProcessor_Specification

IBM created an alternative method:
https://en.wikipedia.org/wiki/OpenPIC_and_MPIC

from years of installing different hardware, drivers, OS,
i can tell that there is a serious problem with intel or Windows or Asus.

Examples:
XPsp3 + 975x Asus P5W DH Deluxe, Q6600, ddr2
works Ok with HD6570 has 2500x1440, 
Digi001 PCI ASIO driver v6.4

same HD6570 and Digi001, 
same drivers,  
same XPsp3 fails on msi X58 Eclipse sli board "Next Gen", x5687, ddr3

Video does Not have 2500x14400 has less options,
Digi001 has completely distorted Audio by the interrupts.

------

other example:

Lynx AES16 PCI driver v19g for W7, v20 for W8.1
installs ok in W7,
does Not install in W8.1 IF the board does Not have MPS1.4
for example:
Asus Rampage III Extreme fails,
has "MPS Adbvanced"
Win8.1 requires MPS1.4
W7x64 works with MPS1.1

but the strange thing is that same Asus board, 
using OSX SnowLeopard 10.6.6 + Bootloader,
installs and works.
Apple claims they only use MPS1.4
but that does Not make any sense.

all very strage.

ASRock works ok, Z370 Pro4
ASUS fails, Rampage III Extreme X58
MSI works ok, X58, Z270 PC Mate
Gigabyte unknown.

--------

other example:

same Lynx AES16, same OS W8.1,
has misplaced buffer sizes,
512 is 256, 256 is 128, 128 is 512, etc...

if installed on AMD boards like:
Tyan S8232

Buffer size can be detected measuring audio latency measuring Analog Input to Analog Output vs. direct path on a Oscilloscope,
from a Y split signal coming from an Audio Signal Generator.

------

i`ve read many claims that PCI is better than USB,
but from my experience, PCI is very unreliable.

there are External PCIe to PCI chasis, like Startech, Magma,
they use Ti IC to Generate MPS1.4 tables and convert to PCIe,
there are 2 versions of the IC,
but is unknown if v1 or v2 has the same problem.

USB seems much more realiable IF the CPU is fast enough.
There is something seriously wrong with ACPI (MPS v1.4 (APIC))
or with Windows.

------

another example:
Sonnet has a 3x PCIe to Thunderbolt3 chassis,
PCB has a small Switch to make some PCIe cards compatible.
like Avid HDX PCIe require that switch.

but other chassis like Razer X Core Chroma work ok, does Not have / Does Not require that switch.
its all very strange.

--------

what other issues have you found?

