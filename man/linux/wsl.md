https://www.linkedin.com/in/alekseirozhkov/
https://github.com/arozhkovru

Windows Subsystem for Linux (WSL) was presenting by Microsoft in 2016. 
It’s a feature of Windows that allows you to run a Linux environment on 
your Windows machine, without the need for a separate virtual machine or dual booting.

Following command should be run with admin rights
```
# Check if WSL installed
dism.exe /online /get-featureinfo /featurename:Microsoft-Windows-Subsystem-Linux
dism.exe /online /get-featureinfo /featurename:VirtualMachinePlatform
# Enable WSL feature in Windows 
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
# Enable WSL version 2 virtual machine
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
# Most usefull WSL management commands
```
# Show all installed WSL images
wsl --list 
# Show online images available for downloading and installing 
wsl --list --online
# Install particulary WSL image from online repository
wsl --install <image-name>
# Delete particular WSL image
wsl --unregister <image-name>
```