The .xml contains the following rules: <br>
<br>
__Registry Persistence : Monitors for common keys used for persistence.<br>
__Program downloaded : Triggers on a specific program anywhere on the system being written to disk, deleted, or renamed.<br>
__New Service Created : Triggers on any new service being created.<br>
__Track a User's Actions : Triggers on a specific user executing, renaming, writing, deleting, reading, or creating a file. This a way to track a user's movement in using HIPs. This is a good rule to apply to privileged accounts.<br>
__Program Execution with a Specific Hash : Triggers on the execution of a specific program with a specific hash.<br>
__Block Specific User's Actions : Blocks all a specific user's actions on a system. This is a decent containment method.<br>
__Changes to System32 : Triggers on anything in System32 bring renamed, written to, or deleted.<br>
__Suspicious DLL : Triggers on any dll being written to the user's appdata folder.<br>
__Execution from User's Temp Folder : Triggers on anything executed in the user's Temp directory.<br>
__Program Execution with the Execption of a Specific User : Triggers on a program being executed with a specific user exclusion.<br>
__Removable Media : Triggers on removable media being attached to the system. McAfee DLP is bettered suited for this but in the absence of it, this work suffices.<br>
__Specific Program Execution Anywhere on System : Triggers on a specific program being executed anywhere on the system. <br>
__Any Program Execution in a Specific Directory : Triggers on a specific program being executed in a specific directory.<br>
