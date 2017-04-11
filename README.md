# VMSnapshotPluginConfig
This repository contains the default VMSnapshotPluginConfig.json file that need to be copied on the VM to be backed up and then configured

The values that needs to be filled for each parameter

1) pluginName - Please don’t change this field
2) preScriptLocation - The absolute path of the pre script
3) postScriptLocation - The absolute path of the post script
4) preScriptParams - This is list of strings. This needs to be populated with parameters that needs to be passed for pre script to execute.
5) postScriptParams - This is list of strings. This needs to be populated with parameters that needs to be passed for post script to execute.
6) preScriptNoOfRetries - Number of retries in case pre-script fails
7) postScriptNoOfRetries - Number of retries that need to be done on in case post-script fails
8) timeoutInSeconds - This is timeout for each script(i.e. pre-script & post-script individually)  to execute for all retires(i.e not for each retry) in seconds. Default is 30.
9) continueBackupOnFailure - This flag makes the backup to continue with file system/crash consistent backup in case of any failures with pre or post script.(i.e. reading,execution,permissions etc)
10) fsFreezeEnabled - This flag can be used to disable fsfreeze command while taking VM snapshot. By default Azure Linux VM Backup will invoke fsfreeze and un-freeze during VM snapshot
