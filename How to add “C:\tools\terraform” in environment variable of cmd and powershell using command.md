How to add “C:\tools\terraform” in environment variable of cmd and powershell using command
# CMD
$ set PATH "%PATH%;C:\tools\terraform";
$ setx PATH "%PATH%;C:\tools\terraform" /M

setx: Command to set environment variables.
PATH: The name of the environment variable you want to modify.
"%PATH%;C:\tools\terraform": Appends the specified directory to the existing PATH variable.
/M: Sets the variable at the system (machine) level.

# Powerpoint
$ [System.Environment]::SetEnvironmentVariable("PATH", $env:PATH + ";C:\tools\terraform", [System.EnvironmentVariableTarget]::Machine)

This PowerShell command appends "C:\tools\terraform" to the existing PATH variable at the machine level.
