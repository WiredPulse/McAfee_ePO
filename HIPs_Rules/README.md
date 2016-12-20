# NOTE
Download the HIPs rules as a zip versus copying and pasting the content or using the right-click and size method. If you do the latter options, there will be formatting issues.
<br><br>
The .xml contains the following rules: <br>
<br>
__Registry Persistence : Monitors for common keys used for persistence.<br><br>
__Unsigned .exe Execution in System32: Triggers on an unsigned executable being ran in system32.<br><br>
__Unsigned .exe Execution: Triggers on an unsigned executable being ran anywhere on the system.<br><br>
__Mounted Drives: Triggers on a drive being mapped.<br><br>
__RDP Invoked: Triggers on RDP being used (mstsc.exe).<br><br>
__Program Execution with a Specific Hash : Triggers on the execution of a specific program with a specific hash.<br><br>
__Program downloaded : Triggers on a specific program anywhere on the system being written to disk, deleted, or renamed.<br><br>
__New Service Created : Triggers on any new service being created.<br><br>
__Track a User's Actions : Triggers on a specific user executing, renaming, writing, deleting, reading, or creating a file. This a way to track a user's movement in using HIPs. This is a good rule to apply to privileged accounts.<br><br>
__Program Execution with the Execption of a Specific User : Triggers on a program being executed with a specific user exclusion.<br><br>
__Block Specific User's Actions : Blocks all a specific user's actions on a system. This is a decent containment method.<br><br>
__Removable Media : Triggers on removable media being attached to the system. McAfee DLP is bettered suited for this but in the absence of it, this work suffices.<br><br>
__Changes to System32 : Triggers on anything in System32 bring renamed, written to, or deleted.<br><br>
__UAC Invoked: Triggers on UAC being invoked (consent.exe)<br><br>
__Program Downloaded, Deleted, or Renamed Anywhere on the System.<br><br>
__Program Execution from User's Temp Folder: Triggers on anything executed in the user's Temp directory.<br><br>
__Application Hooking: Triggers on application hooking other applications:<br><br>
__Open Files from User's Temp Folder: Triggers on any file opening in the user's Temp directory.<br><br>
