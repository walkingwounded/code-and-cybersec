## Windows Updates

cmd: control /name Microsoft.WindowsUpdate

As of Windows 10 onwards, Microsoft windows updates can no longer be ignored. The updates can only be set as postpone. 
This updates are essential to patch vulnerabilities in windows.

## Windows Defender Firewall

The security guard that checks incoming and outgoing personnel and restrict unauthorized personnel from entering or leaving.

cmd: WF.MSC

## Bitlocker

BitLocker provides maximum protection when used with a Trusted Platform Module (TPM), which is a common hardware component installed on Windows devices. The TPM works with BitLocker to ensure that a device hasn't been tampered with while the system is offline.

On devices that don't have a TPM, BitLocker can still be used to encrypt the operating system drive. This implementation requires the user to either:

use a startup key, which is a file stored on a removable drive that is used to start the device, or when resuming from hibernation
use a password. This option isn't secure since it's subject to brute force attacks as there isn't a password lockout logic. As such, the password option is discouraged and disabled by default
Both options don't provide the preboot system integrity verification offered by BitLocker with a TPM.

## Further Studies and Research
Antimalware Scan Interface (AMSI): https://learn.microsoft.com/en-us/windows/win32/amsi/antimalware-scan-interface-portal

Configure Credential Guard: https://learn.microsoft.com/en-us/windows/security/identity-protection/credential-guard/configure?tabs=intune

Configure Windows Hello: https://support.microsoft.com/en-us/windows/configure-windows-hello-dae28983-8242-bb2a-d3d1-87c9d265a5f0#:~:text=Windows%2010,in%20with%20just%20your%20PIN.

Summary Blogpost "Best new Windows 10 security features: Improvements to Intune, Windows Defender Application Guard": https://www.csoonline.com/article/564531/the-best-new-windows-10-security-features.html

Living Off The Land Binaries, Scripts and Libraries: https://lolbas-project.github.io/
