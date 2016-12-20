# NOTE:
Download the McAfee_ePO repository as a whole versus using the copy and paste method or using the right-click and save method. If you do either of the latter two options, there will be formatting issues. 
<br><br>

# Importing Rules into VSE:
1) Download the McAfee_ePO repository<br>
2) Unzip the respository<br>
3) Navigate and log into the McAfee ePO web console<br>
4) Click Menu -> Policy -> Policy Catalog<br>
5) Click 'Import'<br>
6) Click 'Choose'and select the Custom_HIPS_Rules.xml file within the McAfee_ePO-master\HIPs_Rules folder <br>
7) Click OK twice<br>
8) Click on the entry labeled "Custom_HIPs_Rules"<br>
9) Under the 'Type' dropdown at the top of the screen, select 'Custom'<br>
10) The custom rules are shown. From here you can adjust them as you see fit. Once done, add the newly add Custom_HIPs_Rules policy to a container within System Tree.<br>

<br><br>
# Rule Contents and Descriptions:
The .xml contains the following rules: <br>
<br>
__Registry Persistence : Monitors for common Keys\Values used for persistence.<br><br>
__Remote Registry Service Started : Triggers on the Remote Registry Service being started<br><br>
__NTP Server Change : Triggers on a system changing its NTP server setting in the Registry. By default, domain joined systems will use the DC as their time source (Type: NT5DS). Workgroup systems use the Internet (Type: NTP).<br><br>
__Unsigned .exe Execution in c:\windows\* : Triggers on an unsigned executable being ran in c:\windows\*.<br><br>
__Unsigned .exe Execution : Triggers on an unsigned executable being ran anywhere on the system.<br><br>
__Mounted Drives : Triggers on a drive being mapped.<br><br>
__RDP Invoked : Triggers on RDP being used (mstsc.exe).<br><br>
__Disabled UAC : Triggers on UAC being disabled in the Registry.<br><br>
__UAC Bypass : Triggers on the following DLLs being written to disk, which could signal a UAC bypass in progress.<br><br>
__Program downloaded : Triggers on a specific program anywhere on the system being written to disk, deleted, or renamed.<br><br>
__New Service Created : Triggers on any new service being created.<br><br>
__Service Startup Mode change : Triggers on any Service Startup Mode changes.<br><br>
__Track a User's Actions : Triggers on a specific user executing, renaming, writing, deleting, reading, or creating a file. This a way to track a user's movement using HIPs. This is a good rule to apply to privileged accounts.<br><br>
__Program Execution with a Specific Hash : Triggers on the execution of a specific program with a specific hash.<br><br>
__Program Execution with the Execption of a Specific User : Triggers on a program being executed with a specific user being excluded.<br><br>
__Block Specific User's Actions : Blocks all a specific user's actions on a system. This is a decent containment method.<br><br>
__Removable Media : Triggers on removable media being attached to the system. McAfee DLP is bettered suited for this but in the absence of it, this suffices.<br><br>
__Changes to System32 : Triggers on anything in System32 bring renamed, written to, or deleted.<br><br>
__UAC Invoked : Triggers on UAC being invoked (consent.exe)<br><br>
__Application Hooking : Triggers on an application hooking another application.<br><br>
__Program Execution from the Temp Folder : Triggers on anything executed in the user's Temp or the C:\windows\tempdirectory.<br><br>
__Open Files from Temp Folder : Triggers on any file opening in the Temp directory.<br><br>
__Accessibility Feature Alteration : Triggers on alteration of sethc.exe or utilman.exe alteration within c:\windows\system32.<br><br>
__Image File Execution Option Additions : Triggers due to a debugger entry in the Registry with no purpose of "debugging", but rather to run another program instead (likely something malicious).<br><br>
__Prefetch Addition : Triggers on any application execution on the system, which is stored in C:\Windows\Prefetch.<br><br>

