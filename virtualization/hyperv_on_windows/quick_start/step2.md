ms.ContentId: 2964B9FA-FBA4-4F8C-BEF2-A3F3E2FEC6E4
title: Step 2: Install Hyper-V on Windows 10

# Install Hyper-V on Windows 10

Hyper-V can be installed on Windows 10 using **Programs and Features** or [Windows Powershell](#Using-the-Get-WindowsOptionalFeature-cmdlet).


## Using Programs and Features
1. Right-click the **Windows** button and then click **Programs and Features**.

  ![](media\programs_and_features.png)
2. Click **Turn Windows features on or off**.

3. Select **Hyper-V**, click **OK**

  ![](media\hyper-v_feature_selected.png)
4. When the installation is finished, you will need  to restart the computer.

  ![](media\restart.png)
  
## Using the Get-WindowsOptionalFeature cmdlet
For more information, see Get-WindowsOptionalFeature and Using PowerShell to Set Up Hyper-V

1. Click on the **Windows** button and search for **Windows PowerShell**. 
2. Right-click on **Windows PowerShell** and then click **Run as Administrator**.
3. At the Windows Powerhshell prompt, type the following and then press the **Enter** key: 
```enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All``` 
4. When the installation is finished, restart the computer. 

## How do I know it installed?
After you restart your computer start the Hyper-V Manager tool. 

1. Click on the **Windows** button and type **Hyper-V**.
2. Click on **Hyper-V Manager** in the list.
3. The Hyper-V Manager application should start.


# Next Step #
[Step 3: Create a virtual switch](step3.md)