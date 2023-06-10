# Fix-Windows-Local-Security-Authority-Protection
The KB5023706 Windows 11 22H2 cumulative update is a security update that was released on March 14, 2023. It includes several improvements and fixes for Windows 11, such as DCOM hardening, Active Directory domain join issue, and File Explorer enhancements. However, some users have reported seeing a warning message that says "Local Security Authority protection is off. Your device may be vulnerable." even though they have enabled LSA Protection in Windows Security.

LSA Protection is a feature that protects the Local Security Authority (LSA) process from code injection attacks. The LSA process handles user authentication and security policies on Windows devices. To enable LSA Protection, you need to go to Windows Security > Device security > Core isolation details and turn on the Memory integrity setting.

According to Microsoft Technical support, the warning message is a technical glitch that does not affect the actual status of LSA Protection. They said that if you have successfully turned on the feature and you are being prompted to restart, you can ignore the message as the feature is ON regardless of the message.

To verify if LSA Protection is working on your device, you can check the System logs under Windows Logs in the Event Viewer. Look for the WinInit event with the following description: "12: LSASS.exe was started as a protected process with level: 4". This means that LSA had started in protected mode when Windows started.

![LSA_protection_error](https://github.com/Sarvagon/Fix-Windows-Local-Security-Protection/assets/63664894/e5fa5c70-c351-4cf9-9a22-2c48759cd91f)

## INSTRUCTIONS to use Fix-Windows-Local-Security-Authority-Protection
1) Download the .zip or .7z file (you will find them in the "releases" section) and place it on your Desktop.

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Authority-Protection/assets/63664894/b665261c-c397-403d-9f26-51d89ccacb1e)

2) Extract the content of the archive by following these steps (in my case I'm using NanaZip, an OpenSource fork of 7-Zip).
- Right clic < NanaZip (or 7-Zip, ...) < Extract to "Local_Security_Protection\ "

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Authority-Protection/assets/63664894/59074b89-0c9f-4f11-a75f-015d42ab5170)

- You should get this :

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Authority-Protection/assets/63664894/b481ba44-0b44-48e9-8d1c-8471a00a8007)

3) Now go in the "Local_Security_Authority_Protection\ " folder (../Local_Security_Authority_Protection).

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Authority-Protection/assets/63664894/9b335fa4-d831-4664-821f-49f0da7fed70)

4) Execute Local_Security_Authority_Protection.bat file as administrator (Right_clic < Execute as Administrator < Yes)

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Authority-Protection/assets/63664894/6f372fbe-5b93-4920-a560-c589fc967e3c)

5) A dialog window to restart your computer will open. Say "yes" (press O)

![image](https://github.com/Sarvagon/Fix-Windows-Local-Security-Authority-Protection/assets/63664894/a6a87987-2e9b-4124-a3d0-a5cca0e4b394)

6) ENJOY !


