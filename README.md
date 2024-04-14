# Windows-Commands
***Essential Windows commands***

*The Windows command line is one of the most powerful utilities on a Windows PC. With it, we can interact with the OS directly and do a lot of things not available in the graphical user interface (GUI).*

** **
** **

__Basic File and Directory Navigation:__

- **dir**: Lists the files and directories in the current directory.

```
C:\Users\dassu\windowsCommands>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands

14-04-2024  06:58 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:57 PM                13 test1.txt
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
               3 File(s)             39 bytes
               2 Dir(s)  108,630,683,648 bytes free
```

- **cd**: Changes the current directory.

Example: cd Documents (changes to the Documents directory)
```
 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:03 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:57 PM                13 test1.txt
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
14-04-2024  07:03 PM    <DIR>          testFolder
               3 File(s)             39 bytes
               3 Dir(s)  108,629,594,112 bytes free

C:\Users\dassu\windowsCommands>cd testFolder

C:\Users\dassu\windowsCommands\testFolder>

C:\Users\dassu\windowsCommands\testFolder>cd ..

C:\Users\dassu\windowsCommands>
```

- **mkdir**: Creates a new directory.

Example: mkdir NewFolder (creates a new folder named "NewFolder")
```
C:\Users\dassu\windowsCommands\testFolder>mkdir NewFolder

C:\Users\dassu\windowsCommands\testFolder>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands\testFolder

14-04-2024  07:08 PM    <DIR>          .
14-04-2024  07:03 PM    <DIR>          ..
14-04-2024  07:08 PM    <DIR>          NewFolder
               0 File(s)              0 bytes
               3 Dir(s)  108,627,693,568 bytes free
```

- **rmdir**: Removes a directory.

Example: rmdir OldFolder (removes the folder named "OldFolder")
```
C:\Users\dassu\windowsCommands\testFolder>rmdir NewFolder

C:\Users\dassu\windowsCommands\testFolder>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands\testFolder

14-04-2024  07:18 PM    <DIR>          .
14-04-2024  07:03 PM    <DIR>          ..
               0 File(s)              0 bytes
               2 Dir(s)  108,617,166,848 bytes free
```

- **del**: Deletes one or more files.

Example: del file.txt (deletes a file named "file.txt")
```
 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:03 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:57 PM                13 test1.txt
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
14-04-2024  07:18 PM    <DIR>          testFolder
               3 File(s)             39 bytes
               3 Dir(s)  108,616,282,112 bytes free

C:\Users\dassu\windowsCommands>del test1.txt

C:\Users\dassu\windowsCommands>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:22 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
14-04-2024  07:18 PM    <DIR>          testFolder
               2 File(s)             26 bytes
               3 Dir(s)  108,616,282,112 bytes free
```

- **copy**: Copies one or more files from one location to another.

Example: copy file1.txt C:\DestinationFolder (copies "file1.txt" to "DestinationFolder")

```
C:\Users\dassu\windowsCommands>copy test2.txt testFolder
        1 file(s) copied.

C:\Users\dassu\windowsCommands>cd testFolder

C:\Users\dassu\windowsCommands\testFolder>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands\testFolder

14-04-2024  07:28 PM    <DIR>          .
14-04-2024  07:22 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
               1 File(s)             13 bytes
               2 Dir(s)  108,623,585,280 bytes free
```

- **move**: Moves one or more files from one location to another.

Example: move file2.txt C:\NewLocation (moves "file2.txt" to "NewLocation")

```
C:\Users\dassu\windowsCommands>move test3.txt testFolder
        1 file(s) moved.

C:\Users\dassu\windowsCommands>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:33 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  07:33 PM    <DIR>          testFolder
               1 File(s)             13 bytes
               3 Dir(s)  108,623,994,880 bytes free

C:\Users\dassu\windowsCommands>cd testFolder

C:\Users\dassu\windowsCommands\testFolder>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands\testFolder

14-04-2024  07:33 PM    <DIR>          .
14-04-2024  07:33 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  06:58 PM                13 test3.txt
               2 File(s)             26 bytes
               2 Dir(s)  108,623,994,880 bytes free
```

- **ren**: Renames a file or directory.

Example: ren oldname.txt newname.txt (renames "oldname.txt" to "newname.txt")

```
 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:33 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:58 PM                13 test2.txt
14-04-2024  07:33 PM    <DIR>          testFolder
               1 File(s)             13 bytes
               3 Dir(s)  108,623,339,520 bytes free

C:\Users\dassu\windowsCommands>ren test2.txt newNamedFile.txt

C:\Users\dassu\windowsCommands>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands

14-04-2024  07:35 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  06:58 PM                13 newNamedFile.txt
14-04-2024  07:33 PM    <DIR>          testFolder
               1 File(s)             13 bytes
               3 Dir(s)  108,623,204,352 bytes free
```

- **cls**: Clears the command prompt screen.

Example: cls

```
C:\Users\dassu\windowsCommands>cls/?
Clears the screen.

CLS
```

- **type** : display the contents of one or more text files directly to the command prompt or to another command by piping its output.

  Example: type myfile.txt

 > Displaying the contents of a single file:
```
C:\Users\dassu\windowsCommands>type newNamedFile.txt
"Hello World"
```

> Displaying the contents of multiple files:
```
C:\Users\dassu\windowsCommands\testFolder>type test2.txt test3.txt

test2.txt


This is test2.txt file

test3.txt


This is test3.txt file
```

> Redirecting the output to another file:
```
C:\Users\dassu\windowsCommands\testFolder>type test1.txt
This is test1.txt file

C:\Users\dassu\windowsCommands\testFolder>type test2.txt > test1.txt

C:\Users\dassu\windowsCommands\testFolder>type test1.txt
This is test2.txt file
```

> Piping the output to another command:
```
C:\Users\dassu\windowsCommands\testFolder>type test1.txt | find "test"
This is test2.txt file
```

> Using wildcards to display multiple files:
```
C:\Users\dassu\windowsCommands\testFolder>type *.txt

test1.txt


This is test1.txt file

test2.txt


This is test2.txt file

test3.txt


This is test3.txt file
```


- **echo**: Displays messages or turns command echoing on or off.

Example: echo Hello, World!

*common uses of the echo command:*

 > *Display a message*: We can use echo followed by the message we want to display.
```
C:\Users\dassu\windowsCommands>echo Hello World
Hello World
```

> *Display environment variables*: You can use echo with the % symbol to display the value of an environment variable.
```
C:\Users\dassu\windowsCommands>echo %userName%
dassu
```

> *Redirect output*: You can use echo with the redirection operators (> or >>) to write text to a file.
```
C:\Users\dassu\windowsCommands>echo "Hello World" > newNamedFile.txt

C:\Users\dassu\windowsCommands>type newNamedFile.txt
"Hello World"

C:\Users\dassu\windowsCommands>echo My name is Supriyo Das >> newNamedFile.txt

C:\Users\dassu\windowsCommands>type newNamedFile.txt
"Hello World"
My name is Supriyo Das
```

- **xcopy**: Copies files and directory trees.

Example: xcopy source_dir destination_dir
```
C:\Users\dassu\windowsCommands>xcopy testFolder test1Folder
Does test1Folder specify a file name
or directory name on the target
(F = file, D = directory)? D
testFolder\test1.txt
testFolder\test2.txt
testFolder\test3.txt
3 File(s) copied

C:\Users\dassu\windowsCommands>dir
 Volume in drive C has no label.
 Volume Serial Number is 5633-654B

 Directory of C:\Users\dassu\windowsCommands

14-04-2024  09:32 PM    <DIR>          .
14-04-2024  06:54 PM    <DIR>          ..
14-04-2024  09:00 PM                41 newNamedFile.txt
14-04-2024  09:32 PM    <DIR>          test1Folder
14-04-2024  08:53 PM    <DIR>          testFolder
               1 File(s)             41 bytes
               4 Dir(s)  108,611,596,288 bytes free
```
** **
** **
__System Management:__

- **tasklist**: Displays a list of currently running processes.

Example: tasklist
```
C:\Users\dassu\windowsCommands>tasklist

Image Name                     PID Session Name        Session#    Mem Usage
========================= ======== ================ =========== ============
System Idle Process              0 Services                   0          8 K
System                           4 Services                   0        144 K
Secure System                   76 Services                   0     24,604 K
Registry                       116 Services                   0     57,292 K
smss.exe                       556 Services                   0      1,252 K
csrss.exe                      948 Services                   0      5,732 K
wininit.exe                    716 Services                   0      6,984 K
services.exe                  1096 Services                   0     11,216 K
LsaIso.exe                    1116 Services                   0      4,152 K
lsass.exe                     1132 Services                   0     32,312 K
svchost.exe                   1264 Services                   0     39,232 K
```

- **taskkill**: Terminates processes by process ID (PID) or image name.

Example: taskkill /PID 1234 or taskkill /IM notepad.exe
```
C:\Users\dassu\windowsCommands>taskkill /PID 9416 /F
SUCCESS: The process with PID 9416 has been terminated.
```

** **
** **

__File and System Information:__

- **ver**: Display operating system version
```
C:\Users\dassu\windowsCommands>ver

Microsoft Windows [Version 10.0.22631.3447]
```

- **systeminfo**: Show detailed system information
```
C:\Users\dassu\windowsCommands>systeminfo

Host Name:                 SUPRIYO
OS Name:                   Microsoft Windows 11 Pro
OS Version:                10.0.22631 N/A Build 22631
OS Manufacturer:           Microsoft Corporation
OS Configuration:          Standalone Workstation
OS Build Type:             Multiprocessor Free
Registered Owner:          das.supriyo07@gmail.com
Registered Organization:
Product ID:                00330-80141-42239-AA894
Original Install Date:     24-09-2022, 10:17:48 AM
System Boot Time:          14-04-2024, 09:37:47 AM
System Manufacturer:       HP
System Model:              HP Laptop 15s-dy3xxx
System Type:               x64-based PC
Processor(s):              1 Processor(s) Installed.
                           [01]: Intel64 Family 6 Model 140 Stepping 1 GenuineIntel ~2995 Mhz
BIOS Version:              Insyde F.63, 24-08-2023
Windows Directory:         C:\WINDOWS
System Directory:          C:\WINDOWS\system32
Boot Device:               \Device\HarddiskVolume5
System Locale:             en-us;English (United States)
Input Locale:              00004009
Time Zone:                 (UTC+05:30) Chennai, Kolkata, Mumbai, New Delhi
Total Physical Memory:     7,949 MB
Available Physical Memory: 799 MB
Virtual Memory: Max Size:  20,237 MB
Virtual Memory: Available: 12,013 MB
Virtual Memory: In Use:    8,224 MB
Page File Location(s):     C:\pagefile.sys
Domain:                    WORKGROUP
Logon Server:              \\SUPRIYO
Hotfix(s):                 5 Hotfix(s) Installed.
                           [01]: KB5036620
                           [02]: KB5012170
                           [03]: KB5027397
                           [04]: KB5036893
                           [05]: KB5037020
Network Card(s):           8 NIC(s) Installed.
                           [01]: Realtek PCIe GbE Family Controller
                                 Connection Name: Ethernet 2
                                 Status:          Media disconnected
                           [02]: VMware Virtual Ethernet Adapter for VMnet1
                                 Connection Name: VMware Network Adapter VMnet1
                                 DHCP Enabled:    No
                                 IP address(es)
                                 [01]: 192.168.139.1
                                 [02]: fe80::ea3d:835b:fc13:79fc
                           [03]: Bluetooth Device (Personal Area Network)
                                 Connection Name: Bluetooth Network Connection
                                 Status:          Media disconnected
                           [04]: VirtualBox Host-Only Ethernet Adapter
                                 Connection Name: Ethernet
                                 DHCP Enabled:    No
                                 IP address(es)
                                 [01]: 192.168.56.1
                                 [02]: fe80::66b3:ed3b:bed6:ca33
                           [05]: VMware Virtual Ethernet Adapter for VMnet8
                                 Connection Name: VMware Network Adapter VMnet8
                                 DHCP Enabled:    No
                                 IP address(es)
                                 [01]: 192.168.254.1
                                 [02]: fe80::3844:72a9:85e2:7963
                           [06]: VirtualBox Host-Only Ethernet Adapter
                                 Connection Name: Ethernet 3
                                 DHCP Enabled:    No
                                 IP address(es)
                                 [01]: 10.0.0.1
                                 [02]: fe80::af6d:dfc7:1aac:3d0f
                           [07]: Realtek RTL8822CE 802.11ac PCIe Adapter
                                 Connection Name: Wi-Fi
                                 DHCP Enabled:    Yes
                                 DHCP Server:     192.168.9.7
                                 IP address(es)
                                 [01]: 192.168.9.229
                                 [02]: fe80::42ce:47c:4db:ce4c
                                 [03]: 2401:4900:627e:eed1:1972:7d9b:cde5:d965
                                 [04]: 2401:4900:627e:eed1:31a3:5e4c:c001:51fc
                           [08]: Microsoft Wi-Fi Direct Virtual Adapter
                                 Connection Name: Local Area Connection* 15
                                 DHCP Enabled:    No
                                 IP address(es)
                                 [01]: 192.168.137.1
                                 [02]: fe80::4755:d6fd:d11b:ab0e
Hyper-V Requirements:      A hypervisor has been detected. Features required for Hyper-V will not be displayed.
```

- **attrib**: View or change file attributes (e.g., hidden, read-only)
```
C:\Users\dassu\windowsCommands>attrib newNamedFile.txt
A                    C:\Users\dassu\windowsCommands\newNamedFile.txt

C:\Users\dassu\windowsCommands>attrib/?
Displays or changes file attributes.

ATTRIB [+R | -R] [+A | -A] [+S | -S] [+H | -H] [+O | -O] [+I | -I] [+X | -X] [+P | -P] [+U | -U]
       [drive:][path][filename] [/S [/D]] [/L]

  +   Sets an attribute.
  -   Clears an attribute.
  R   Read-only file attribute.
  A   Archive file attribute.
  S   System file attribute.
  H   Hidden file attribute.
  O   Offline attribute.
  I   Not content indexed file attribute.
  X   No scrub file attribute.
  V   Integrity attribute.
  P   Pinned attribute.
  U   Unpinned attribute.
  B   SMR Blob attribute.
  [drive:][path][filename]
      Specifies a file or files for attrib to process.
  /S  Processes matching files in the current folder
      and all subfolders.
  /D  Processes folders as well.
  /L  Work on the attributes of the Symbolic Link versus
      the target of the Symbolic Link
```

- **where**: Locate executable files
```
C:\Users\dassu\windowsCommands>where *.txt
C:\Users\dassu\windowsCommands\newNamedFile.txt
C:\Users\dassu\AppData\Local\Programs\Python\Python311\LICENSE.txt
C:\Users\dassu\AppData\Local\Programs\Python\Python311\NEWS.txt
C:\Windows\System32\ThirdPartyNoticesBySHS.txt
C:\Windows\System32\VmFirmware Third-Party Notices.txt
C:\Windows\System32\VmFirmwareHcl Third-Party Notices.txt
C:\Program Files\PuTTY\README.txt
C:\ProgramData\chocolatey\bin\_processed.txt
C:\Program Files\PowerShell\7\LICENSE.txt
C:\Program Files\PowerShell\7\ThirdPartyNotices.txt
```

** **
** **

__Network and Connectivity:__

- **ipconfig**: Display network adapter configuration
```
C:\Users\dassu\windowsCommands>ipconfig

Windows IP Configuration


Ethernet adapter Ethernet 2:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Ethernet adapter Ethernet:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : f**0::66**:ed3b:****:c**3%19
   IPv4 Address. . . . . . . . . . . : 192.1**.**.*
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :

Ethernet adapter Ethernet 3:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : f**0::**6d:df*7:***c:3**f%18
   IPv4 Address. . . . . . . . . . . : 10.0.0.1
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :

Wireless LAN adapter Local Area Connection* 12:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 15:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : ***0::4***:d**d:d11b:****%7
   IPv4 Address. . . . . . . . . . . : 192.168.***.1
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :

Ethernet adapter VMware Network Adapter VMnet1:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : f**0::e**d:**5b:f***:***c%8
   IPv4 Address. . . . . . . . . . . : 192.168.***.1
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :

Ethernet adapter VMware Network Adapter VMnet8:

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : ****::****:****:****:***3%6
   IPv4 Address. . . . . . . . . . . : 192.168.***.*
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . :
   IPv6 Address. . . . . . . . . . . : ****:****:****:****:****:5e4c:c001:****
   Temporary IPv6 Address. . . . . . : ****:****:627e:eed1:****:7d9b:****:d965
   Link-local IPv6 Address . . . . . : f***::**ce:4**:**b:****%11
   IPv4 Address. . . . . . . . . . . : 192.168.*.***
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : f**0::****:beff:****:****%11
                                       192.***.**.*

Ethernet adapter Bluetooth Network Connection:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Ethernet adapter vEthernet (Default Switch):

   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : f***::****:***a:****:cd7e%28
   IPv4 Address. . . . . . . . . . . : 172.**.1**.*
   Subnet Mask . . . . . . . . . . . : 255.255.***.0
   Default Gateway . . . . . . . . . :
```
- **ping**: Test network connectivity to a host (e.g., ping google.com)
```
C:\Users\dassu\windowsCommands>ping 127.0.0.1

Pinging 127.0.0.1 with 32 bytes of data:
Reply from 127.0.0.1: bytes=32 time<1ms TTL=128
Reply from 127.0.0.1: bytes=32 time<1ms TTL=128
Reply from 127.0.0.1: bytes=32 time<1ms TTL=128
Reply from 127.0.0.1: bytes=32 time<1ms TTL=128

Ping statistics for 127.0.0.1:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms

C:\Users\dassu\windowsCommands>ping www.google.com

Pinging www.google.com [2404:6800:4007:81a::2004] with 32 bytes of data:
Reply from 2404:6800:4007:81a::2004: time=25ms
Reply from 2404:6800:4007:81a::2004: time=36ms
Reply from 2404:6800:4007:81a::2004: time=31ms
Reply from 2404:6800:4007:81a::2004: time=44ms

Ping statistics for 2404:6800:4007:81a::2004:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 25ms, Maximum = 44ms, Average = 34ms
```

- **tracert**: Trace the route to a host (network troubleshooting)
```
C:\Users\dassu\windowsCommands>tracert www.google.com

Tracing route to www.google.com [2404:6800:4007:81a::2004]
over a maximum of 30 hops:

  1    14 ms     4 ms     2 ms  2401:4900:627e:eed1::a0
  2     *        *        *     Request timed out.
  3    37 ms    30 ms    45 ms  2401:4900:c4:46c1::1
  4     *       64 ms    23 ms  2401:4900:0:6f9::3
  5    43 ms    30 ms    26 ms  2401:4900:0:6f9::1
  6     *        *        *     Request timed out.
  7    51 ms    37 ms    48 ms  2404:a800:3a00:1::4c5
  8     *        *        *     Request timed out.
  9    51 ms    35 ms    22 ms  2001:4860:1:1::674
 10    27 ms    35 ms    30 ms  2404:6800:809a::1
 11    57 ms    27 ms    28 ms  2001:4860:0:1::ac6
 12    51 ms    25 ms    59 ms  2001:4860:0:1::8808
 13    36 ms    41 ms    23 ms  2001:4860:0:1::40e9
 14    44 ms    50 ms    29 ms  2001:4860:0:1::565d
 15    50 ms    35 ms    26 ms  maa05s19-in-x04.1e100.net [2404:6800:4007:81a::2004]

Trace complete.
```

- **netsh**: Configure network settings (advanced)
```
C:\Users\dassu\windowsCommands>netsh interface show interface

Admin State    State          Type             Interface Name
-------------------------------------------------------------------------
Enabled        Disconnected   Dedicated        Ethernet 2
Enabled        Connected      Dedicated        Ethernet
Enabled        Connected      Dedicated        Ethernet 3
Enabled        Connected      Dedicated        VMware Network Adapter VMnet1
Enabled        Connected      Dedicated        VMware Network Adapter VMnet8
Enabled        Connected      Dedicated        Wi-Fi
Enabled        Connected      Dedicated        Local Area Connection* 15

C:\Users\dassu\windowsCommands>netsh interface ip show config

Configuration for interface "Ethernet 2"
    DHCP enabled:                         Yes
    InterfaceMetric:                      5
    DNS servers configured through DHCP:  None
    Register with which suffix:           Primary only
    WINS servers configured through DHCP: None

Configuration for interface "Ethernet"
    DHCP enabled:                         No
    IP Address:                           ***.***.**.*
    Subnet Prefix:                        ***.***.**.0/** (mask 255.2**.***.*)
    InterfaceMetric:                      25
    Statically Configured DNS Servers:    None
    Register with which suffix:           Primary only
    Statically Configured WINS Servers:   None

Configuration for interface "Ethernet 3"
    DHCP enabled:                         No
    IP Address:                           10.0.0.1
    Subnet Prefix:                        10.0.0.0/24 (mask 255.255.255.0)
    InterfaceMetric:                      25
    Statically Configured DNS Servers:    None
    Register with which suffix:           Primary only
    Statically Configured WINS Servers:   None

Configuration for interface "Local Area Connection* 12"
    DHCP enabled:                         Yes
    InterfaceMetric:                      25
    DNS servers configured through DHCP:  None
    Register with which suffix:           Primary only
    WINS servers configured through DHCP: None

Configuration for interface "Local Area Connection* 15"
    DHCP enabled:                         No
    IP Address:                           ***.***.***.*
    Subnet Prefix:                        ***.***.***.0/** (mask 255.2**.***.*)
    InterfaceMetric:                      25
    Statically Configured DNS Servers:    None
    Register with which suffix:           Primary only
    Statically Configured WINS Servers:   None

Configuration for interface "VMware Network Adapter VMnet1"
    DHCP enabled:                         No
    IP Address:                           ***.***.***.*
    Subnet Prefix:                        ***.***.***.0/** (mask 255.2**.***.*)
    InterfaceMetric:                      35
    Statically Configured DNS Servers:    None
    Register with which suffix:           Primary only
    Statically Configured WINS Servers:   None

Configuration for interface "VMware Network Adapter VMnet8"
    DHCP enabled:                         No
    IP Address:                           ***.***.***.*
    Subnet Prefix:                        ***.***.***.0/** (mask 255.2**.***.*)
    InterfaceMetric:                      35
    Statically Configured DNS Servers:    None
    Register with which suffix:           Primary only
    Statically Configured WINS Servers:   None

Configuration for interface "Wi-Fi"
    DHCP enabled:                         Yes
    IP Address:                           ***.***.*.***
    Subnet Prefix:                        ***.***.*.0/** (mask 255.2**.***.*)
    Default Gateway:                      ***.***.*.*
    Gateway Metric:                       0
    InterfaceMetric:                      **
    DNS servers configured through DHCP:  ***.***.*.*
    Register with which suffix:           Primary only
    WINS servers configured through DHCP: None

Configuration for interface "Bluetooth Network Connection"
    DHCP enabled:                         Yes
    InterfaceMetric:                      65
    DNS servers configured through DHCP:  None
    Register with which suffix:           Primary only
    WINS servers configured through DHCP: None

Configuration for interface "Loopback Pseudo-Interface 1"
    DHCP enabled:                         No
    IP Address:                           127.0.0.1
    Subnet Prefix:                        127.0.0.0/* (mask 255.0.0.0)
    InterfaceMetric:                      75
    Statically Configured DNS Servers:    None
    Register with which suffix:           Primary only
    Statically Configured WINS Servers:   None

Configuration for interface "vEthernet (Default Switch)"
    DHCP enabled:                         No
    IP Address:                           ***.29.***.1
    Subnet Prefix:                        ***.29.***.0/** (mask 255.2**.***.*)
    InterfaceMetric:                      ****
    Statically Configured DNS Servers:    None
    Register with which suffix:           None
    Statically Configured WINS Servers:   None
```

   **shutdown**: Shut down or restart the computer (e.g., shutdown /s /t 60 - shuts down in 60 seconds)
   ** **
   ** **
   __User Management:__

- **net user**: Manage user accounts (add, remove, modify)
```
C:\Users\dassu\windowsCommands>net user

User accounts for \\SUPRIYO

-------------------------------------------------------------------------------
Administrator            dassu                    DefaultAccount
Guest                    WDAGUtilityAccount
The command completed successfully.
```

- **whoami**: Display the current user name
```
C:\Users\dassu\windowsCommands>whoami
supriyo\dassu
```
** **
** **
