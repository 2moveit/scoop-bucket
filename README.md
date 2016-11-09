# scoop-bucket
Repository for apps to install via [Scoop](http://scoop.sh/).

1. If you do not like the default installation path  `~\appdata\local\scoop\` you can set path for the apps with an environment variable in Powershell 3. Do this before the installation or you'll have to uninstall scoop first. `[environment]::setEnvironmentVariable('SCOOP','D:\Scoop-Apps','User')`

2. Install Scoop with Powershell 3:
`iex (new-object net.webclient).downloadstring('https://get.scoop.sh')`

3. You might need to change the execution policy (i.e. enable Powershell): 
`set-executionpolicy unrestricted -s cu`

4. To add this bucket repsitory: `scoop bucket add 2moveit https://github.com/2moveit/scoop-bucket`

5. Check if the bucket is installed: `scoop bucket list # -> you should see 2moveit`

6. `scoop search` to list all apps (also from main bucket)

7. `scoop install <appname>`to install an app
