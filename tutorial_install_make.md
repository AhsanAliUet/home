## How to install ```make``` (for Makefiles) command in Windows?  

Here are the steps:  
1. Press Windows or start button and search for PowerShell and open it as administrator.  
2. Run the command ```Get-ExecutionPolicy```. If you see **Restricted**, the run ```Set-ExecutionPolicy AllSigned``` or ```Set-ExecutionPolicy Bypass -Scope Process```  
3. In the 3rd step, run the following command:  
```Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))```   