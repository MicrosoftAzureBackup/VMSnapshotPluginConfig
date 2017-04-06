# VMSnapshotPluginConfig
This repository contains the default VMSnapshotPluginConfig.json file that need to be copied on the VM to be backed up and then configured

The values that needs to be filled for each parameter

1) pluginName - The name of the plugin which by default is "ScriptRunner" (Better dont edit this parameter)
2) preScriptLocation - The absolute path of the pre script
3) postScriptLocation - The absolute path of the post script
4) preScriptParams - This is list of strings. This needs to be populated with parameters that needs to be passed for pre script to execute.
5) postScriptParams - This is list of strings. This needs to be populated with parameters that needs to be passed for post script to execute.
6) preScriptNoOfRetries - Number of retries that need to be done on failure of pre script
7) postScriptNoOfRetries -  Number of retries that need to be done on failure of post script
8) timeoutInSeconds - This is timeout for each script to execute for all retires(i.e not for each retry) in seconds. Default is 30.
9) continueBackupOnFailure - This flag makes the backup to continue when there is failure with scripts(i.e. reading,execution,permissions etc) with "filesystem consistent backup" when set true. Default is true.
10) fsFreezeEnabled - file system will be frozen and unfrozen before and after taking the snapshots respcetively when this flag is set true. Default is true.
