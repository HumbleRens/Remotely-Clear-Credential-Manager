# Remotely Clear Windows Credential Manager
The script first prompts for the administrator password of each remote computer using Get-Credential. It creates a new PSSession to each remote computer and runs a ScriptBlock that uses the cmdkey command to list all stored credentials and deletes them one by one.

You will need to replace the $computers variable with the names of the remote computers you want to run this script on. It will remove all saved credentials on a computer.
