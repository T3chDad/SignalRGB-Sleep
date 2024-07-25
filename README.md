# SignalRGB-Sleep
Even though there are options in SignalRGB for turning off lighting when the computer/monitor sleeps or locks, it appears that many (including me) cannot get this function to work whatsoever.

This seems to be a long standing issue and I'm impatient and OCD, so this is my attempt at a kludge to create more reliable sleep (lights-out) functionality via an open source windows utility. This is largely just an excersize to dust off my Google, Stack Overflow, and YouTube coding certifications. :D  I'm sharing this application in case anyone else would like to have this functionality to SignalRGB without too much trouble. No installation is needed. Just download the zip and extract it somewhere on your system that has SignalRGB installed and run the `"signalRGB-Sleep.exe"`.

This app is essentially a proof of concept and should not be considered a production worthy release and likely has bugs. It was authored in VS2022 in C# under .NET Core 8.0. It functions as a GUI wrapper between the SignalRGB command line capability and detecting the different idle/lock states of the computer. When the program detects a lock or idle timeout, it uses the shell to tell SignalRGB to change to the desired "OFF" effect. When it detects a wake or unlock event, it tells SignalRGB to change to the desired "ON" effect...simple right?!

For Example:  
--The default sleep effect is "Solid Color" with the settings of Black and 0 brightness.  
--The default wake effect is "Screen Ambience". 

You can change the desired effects in the app settings (double-click tray/notification area icon). The effects you specify must already be installed and configured with SignalRGB itself. You need to ensure the effect names specified here must match the names in the SignalRGB interface. Spaces are supported.

![signalRGB-Sleep_jVM1ddahcj](https://github.com/user-attachments/assets/6e270cb2-40b1-4c1a-8cf5-c27f602e8de3)

If you enjoy this project or I have helped you in some way...please feel free to [buy me a coffee](https://www.buymeacoffee.com/hVmOfsXjX1).
************************************************************************************************
Use this program at your own risk. I'm not responsible for anything that happens on your system.
************************************************************************************************


