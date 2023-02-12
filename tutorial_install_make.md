## How to install ```make``` (for Makefiles) command in Windows?  

Here are the steps:  
1. Press Windows or start button and search for PowerShell and open it as administrator.  
2. Run the command ```Get-ExecutionPolicy```. If you see **Restricted**, the run ```Set-ExecutionPolicy AllSigned``` or ```Set-ExecutionPolicy Bypass -Scope Process```  
3. In the 3rd step, run the following command:  
```Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))```   

4. Wait for the command to be completed. If there are no errors found, you have installed choco in your computer. Otherwise, search for the errors, resolve them and again run the step 3.  

5. In the final step, run the following command:   
```choco install make```  

Wait for the above command to be completed. If it ran successfully, you have installed ```make``` command in your computer. Close the PowerShell and again open it. Run the command ```make --version```. Make sure there are no errors now.  

Enjoy it :)