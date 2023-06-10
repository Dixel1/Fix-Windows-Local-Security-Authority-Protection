# Fix-Windows-Local-Security-Protection
While Windows users report that this issue is caused by the recently released KB5023706 Windows 11 22H2 cumulative update, this has been happening since at least January 15.

The "Local Security Authority protection is off. Your device may be vulnerable." warnings show up even though LSA Protection is enabled in Windows Security > Device security > Core isolation details.

"There is a technical glitch with this feature, if you have successfully turned on this feature and you are being prompted to restart, kindly note that the feature is ON irrespective of the message as this is a technical glitch that we are aware of and we are working to resolve that issue soonest," Microsoft Technical support representative reportedly told one of the affected users.

To check if LSA had actually started in protected mode on your computer when Windows started, you can search for the following WinInit event in the System logs under Windows Logs: "12: LSASS.exe was started as a protected process with level: 4"

![LSA_protection_error](https://github.com/Sarvagon/Fix-Windows-Local-Security-Protection/assets/63664894/e5fa5c70-c351-4cf9-9a22-2c48759cd91f)

## INSTRUCTIONS to use Fix-Windows-Local-Security-Protection :
1) Download the .zip or .7z file (you will find them in the "releases" section) and place it on your Desktop.
2) 
![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Protection/assets/63664894/f37ce1f6-0ba7-41a1-8b40-98801d8b1826)

2) Extract the content of the archive by following these steps (in my case I'm using NanaZip, an OpenSource fork of 7-Zip).
- Right clic < NanaZip (or 7-Zip, ...) < Extract to "Local_Security_Protection\ "

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Protection/assets/63664894/bf20a71b-0945-4717-9667-6776259b172b)

- You should get this :

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Protection/assets/63664894/415ebde0-5153-4fbc-b2d8-66322197fabc)

3) Now go in the "Local_Security_Protection\ " folder (../Local_Security_Protection).

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Protection/assets/63664894/34ecc9cd-7400-466e-9984-064baf9617d5)

4) Execute Local_Security_Protection.bat file as administrator (Right_clic < Execute as Administrator)

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Protection/assets/63664894/469db56c-3484-4637-86a2-37b4052c2e26)

5) A dialog window to restart your computer will open. Say "yes" (press O)

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Protection/assets/63664894/d1486c10-a954-4f30-aaff-42b6948c696a)

6) ENJOY !


