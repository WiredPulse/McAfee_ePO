# NOTE:
Download the McAfee_ePO repository as a whole versus using the copy and paste method or using the right-click and save method. If you do either of the latter two options, there will be formatting issues. 
<br><br>

# Importing Rules into VSE:
1) Download the McAfee_ePO repository<br>
2) Unzip the respository<br>
3) Navigate to the McAfee ePO web console and log in<br>
4) Click Menu -> Policy -> Policy Catalog<br>
5) Select VirusScan Enterprise within the Product drop-down<br>
5) Click 'Import'<br>
6) Click 'Choose' and select the Custom_Custom_User-Defined_Rules.xml file within the McAfee_ePO-master\VSE_User-Defined_Rules folder <br>
7) Click OK twice<br>
8) Click on the entry labeled "Custom_User-Defined_Rules"<br>
9) Click User-Defined Rules under Categories to see the rules<br>
<br>
The custom rules are identical for Workstation and Server. No other rules are enabled but the custom ones and they are all set to log only. <br>

# Rules:
RDP Port Detection (Lateral Movement) <br><br>
New Service Created (Persistence OR Priv. Escalation) <br><br>
Removable Media Attached (C2 OR Exfil.) <br><br>
RDP Invoked (Lateral Movement OR Execution) <br><br>
UAC Invoked (Priv. Escalation OR Execution) <br><br>
Mounted Drive (Lateral Movement OR Exfil.) <br><br>
UTILMAN.exe Alteration (Persistence OR Priv. Escalation) <br><br>
SETHC.exe Alteration (Persistence OR Priv. Escalation) <br><br>
Image File Execution Key Change (Persistence OR Priv. Escalation) <br><br>
RUNDLL32.exe (Defense Evasion OR Execution) <br><br>
ARP.exe (Host Enumeration OR Execution) <br><br>
VNC Port Detection (Lateral Movement) <br><br>
NBTSTAT.exe (Host Enumeration OR Execution) <br><br>
WMIC.exe (Host Enumeration OR Execution) <br><br>
CMD.exe (Lateral Movement or Execution) <br><br>
7z.exe (Execution OR Exfil) <br><br>
SC.exe (Persistence) <br><br>
AT.exe (Persistence, Priv. Escalation, Execution OR Exfil.) <br><br>
NET Command (Host Enumeration OR Execution) <br><br>
NETSTAT.exe (Host Enumeration OR Execution) <br><br>
MSIEXEC.exe (Persistence OR Execution) <br><br>
PSEXEC.exe (Lateral Movement, Execution, or Exfil.) <br><br>
TeamViewer Port Detection (Lateral Movement) <br><br>
DSQUERY.exe (Host Enumeration OR Execution) <br><br>
TASKLIST.exe (Host Enumeration OR Execution) <br><br>
TASKKILL.exe (Defense Evasion OR Execution) <br><br>
SYSTEMINFO.exe (Host Enumeration OR Execution) <br><br>
XCOPY.exe (Execution OR Exfil.) <br><br>
POWERSHELL.exe (Lateral Movement, Host Enumeration OR Execution) <br><br>
REG ADD or REG QUERY Use (Persistence, Defense Evasion, Host Enumeration, OR Execution) <br><br>
QUSER.exe (Host Enumeration OR Execution) <br><br>
WINRAR.exe (Execution OR Exfil.) <br><br>
ROUTE.exe (Host Enumeration, Lateral Movement, OR Execution) <br><br>
SMB Port Detection (Lateral Movement) <br><br>
AppInit_DLLs Value Change (Persistence, Priv. Escalation, OR Defense Evasion) <br><br>
UAC Bypass - CRYPTBASE.dll (Priv. Escalation) <br><br>
UAC Bypass - SHCORE.dll (Priv. Escalation) <br><br>
UAC Bypass - WDSCORE.dll (Priv. Escalation) <br><br>
UAC Bypass - ActionQueue.dll (Priv. Escalation) <br><br>
UAC Bypass - NTWDBLIB.dll (Priv. Escalation) <br><br>
HIPS Rules Dumped (Defense Evasion) <br><br>
Folder Watch<br><br>
Prefetch Watch (Execution) <br><br>
NTP Server Change (Defense Evasion) <br><br>
Service Startup Mode Change (Persistence OR Priv. Escalation) <br><br>
Disable UAC (Priv. Escalation OR Defense Evasion) <br><br>
VBS Use (Host Enumeration OR Lateral Movement) <br><br>
Data in $recycle.bin (exfil.) <br><br>
MSHTA.exe execution (Lateral Movement OR Execution)<br><br>
Disabling Volume Shadow Copy Service (Defense Evasion)<br><br>
PowerShell Profile Addition (Persistence)<br><br>
