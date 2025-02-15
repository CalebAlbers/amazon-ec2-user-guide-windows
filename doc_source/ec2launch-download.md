# Install the latest version of EC2Launch<a name="ec2launch-download"></a>

Use the following procedure to download and install the latest version of EC2Launch on your instances\.

**To download and install the latest version of EC2Launch**

1. If you have already installed and configured EC2Launch on an instance, make a backup of the EC2Launch configuration file\. The installation process does not preserve changes in this file\. By default, the file is located in the `C:\ProgramData\Amazon\EC2-Windows\Launch\Config` directory\.

1. Download [EC2\-Windows\-Launch\.zip](https://s3.amazonaws.com/ec2-downloads-windows/EC2Launch/latest/EC2-Windows-Launch.zip) to a directory on the instance\.

1. Download [install\.ps1](https://s3.amazonaws.com/ec2-downloads-windows/EC2Launch/latest/install.ps1) to the same directory where you downloaded `EC2-Windows-Launch.zip`\.

1. Run `install.ps1`

1. If you made a backup of the EC2Launch configuration file, copy it to the `C:\ProgramData\Amazon\EC2-Windows\Launch\Config` directory\.

**To download and install the latest version of EC2Launch using PowerShell**  
If you have already installed and configured EC2Launch on an instance, make a backup of the EC2Launch configuration file\. The installation process does not preserve changes in this file\. By default, the file is located in the `C:\ProgramData\Amazon\EC2-Windows\Launch\Config` directory\.

To install the latest version of EC2Launch using PowerShell, run the following commands from a PowerShell window

```
mkdir $env:USERPROFILE\Desktop\EC2Launch
$Url = "https://s3.amazonaws.com/ec2-downloads-windows/EC2Launch/latest/EC2-Windows-Launch.zip"
$DownloadZipFile = "$env:USERPROFILE\Desktop\EC2Launch\" + $(Split-Path -Path $Url -Leaf)
Invoke-WebRequest -Uri $Url -OutFile $DownloadZipFile
$Url = "https://s3.amazonaws.com/ec2-downloads-windows/EC2Launch/latest/install.ps1"
$DownloadZipFile = "$env:USERPROFILE\Desktop\EC2Launch\" + $(Split-Path -Path $Url -Leaf)
Invoke-WebRequest -Uri $Url -OutFile $DownloadZipFile
C:\Users\Administrator\Desktop\EC2Launch\install.ps1
```

Verify the installation by checking `C:\ProgramData\Amazon\EC2-Windows\Launch`\.