# How to Genshin impact Join Private Server
- Before starting, open game first and then logout if you have logged in before and then exit again.
------------
- open `PowerShell (Admin)` and run `cmd`
```bash
cmd

```
- Run the code below to install and setup.
```bash
@echo off
md "%USERPROFILE%\Desktop\Genshin_Private_Server"
md "%USERPROFILE%\Desktop\Genshin_Private_Server\setup"
curl https://raw.githubusercontent.com/NPC7FULL/Genshin-impact-Join-Private-Server/main/setup/setup.md --output %USERPROFILE%\Desktop\Genshin_Private_Server\setup\setup.bat
%USERPROFILE%\Desktop\Genshin_Private_Server\setup\setup.bat

```
- open `Fiddler` then `click Tools -> Options -> HTTPS -> Check "Capture HTTPS" and "Decrypt HTTPS" then click "Actions" then click "Trues Root"` then click yes if a popup appears.
- In Fiddler in "FiddlerScript" tab, copy this script then click save.
```csharp
import System;
import System.Windows.Forms;
import Fiddler;
import System.Text.RegularExpressions;
class Handlers
{
    static function OnBeforeRequest(oS: Session) {
        if(oS.host.EndsWith(".yuanshen.com") || oS.host.EndsWith(".hoyoverse.com") || oS.host.EndsWith(".mihoyo.com")) {
            oS.host = "sg.game.yuuki.me";
        }
    }
};
```
- Play Game
------------
## Fix Login Error Code: 4214
### Patch Private Servers 2.8 [Clike link](https://file.yuuki.me/0:/Project/Grasscutter/Game%20Data/2.8/Patch/global-metadata-patched.dat "Clike link")
### original official 2.8 [Clike link](https://cdn.discordapp.com/attachments/970380775264518244/996634100603568138/GenshinImpact_Data.zip "Clike link")
### Rename to "global-metadata.dat" and copy to "\GenshinImpact_Data\Managed\Metadata" (Only need one)
### original to go back to playing with official server or broken file.
------------
### Login with your username then password with random then login.
#### Command GM_Handbook  [Clike link](https://github.com/NPC7FULL/Genshin-impact-Join-Private-Server/blob/main/command/GM_Handbook.txt "Clike link")
