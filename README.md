# A2osX
Multi-Tasking OS for Apple II
## Requires :
Enh IIe (65c02 cpu) with 128k, //c, IIgs
## General Information:
**A2OSX.BOOT.DSK** : 140k A2osX boot disk will all binaries  
**A2OSX.SRC.po** : 800k S-C MASM boot disk with all sources  
  
OApple+1,OApple+2,OApple+3 to switch between screens : Kernel Log, text, DHGR.  
(OApple+shift+1,OApple+shift+2,OApple+shift+3 on FR keyboard)  
  
### **** Developers WANTED ****  

!!! Help on writing this code should be greatly appreciated !!!  

...
In Progress : moving TCPIP to some soket API
In Progress : moving KERNEL to AuxLC Bnk1 & 2 (16k, more space for drivers)
...

## SYS/KM* Supported Hardware At Kernel Level (ProDOS):
| KM.Name | Status | Comment |
| ------- | ------ | ------- |
| KM.NSC | Working | No-Slot-Clock |
| KM.RAMWORKS | Working | AE-Ramworks I,II,III |
  
## SBIN,Daemons:  
| Name.DRV | Status | Comment |
| -------- | ------ | ------- |
| INSDEV | Working | |
| GETTY | Working | |
| LOGIN | In Progress | no auth using /etc/passd yet |
| TCPIP | In Progress | |
| DHCPCLNT | Working | |
| SHELL | Working | BUG: History nav|
  
## DRV,Drivers:  
| Name.DRV | Status | Comment |
| -------- | ------ | ------- |
| Console.DRV | Working | ANSI support in Progress. |
| PPIC.DRV | In Progress | |
| SSC.DRV | In Progress | |
| SSC.I.DRV | In Progress | |
| Mouse.DRV | Working | |
| Uthernet.DRV | Working | |
| UthernetII.DRV | In Progress | |
| LanCeGS.DRV | In Progress | |
| Mouse.DRV | Working | |
| DHGR.DRV | In Progress | except bitblt... |
  
## Internal Shell commands:  
| Name | Status | Comment |
| ---- | ------ | ------- |
| CD | Working | |
| DATE | Working  | |
| ECHO | Working | |
| EXIT | Working  | |
| PAUSE | Working | |
| TIME | Working  | |
| TYPE | Working  | |
| SET | Working  | |
| STARTPROC | Working  | Used in A2osX.startup |
  
## BIN,External Shell commands:  
| Name | Status | Comment |
| ---- | ------ | ------- |
| MEM | Working | |
| LSDEV | Working | |
| PS | Working | |
| MD | Working | |
| RM | Working | |
| LS | Working  | BUG: `ls dir` does not list dir content (`ls dir/` works) |
| CP | | |
| ARP | Working | |
| PING | Working | |
| DNSINFO | In Progress | |
| IPCONFIG | Working | renamed from NETINFO |
| NETSTAT | Working | |
| RPCDUMP | In Progress | tool based on UDP socket API, renamed from RPCINFO |
| EDIT | Working | still missing : find/replace |
| NSCUTIL | Working | Tool for setting time in NSC/DL1216E |
| ASM | In Progress | S-C MASM based multi CPU assembler |
  
## Misc  
### S-C MASM color scheme for Notepad++  
...drop _Tools/userDefineLang.xml in %APPDATA%\Notepad++  
;-)

