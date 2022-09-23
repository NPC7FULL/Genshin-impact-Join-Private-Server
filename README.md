# How to Genshin impact Join Private Server New 3.0
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
        if(oS.host.EndsWith(".yuanshen.com") || oS.host.EndsWith(".hoyoverse.com") || oS.host.EndsWith(".mihoyo.com") || oS.uriContains("http://overseauspider.yuanshen.com:8888/log")) {
            //New Update 3.0
            oS.host = "sg.genshin.ps.yuuki.me";
        }
    }
};
```
- Play Game
------------
## Fix Login Error Code: 4214
### Patch Private Servers 3.0 [Clike link](https://mega.nz/file/Gv42Sb5R#_QwwSROMBO0Bk_wofLrTqR48x68PhhtD0Ld8ImniJUE "Clike link")
### original official 3.0 [Clike link](https://mega.nz/file/6r4lCYwS#XJVXeFV9In894Ropd3LRnDa7fUmna3JR459kfkGKuKk "Clike link")
#### Rename to "global-metadata.dat" and copy to "Genshin Impact game\GenshinImpact_Data\Managed\Metadata"
#### original to go back to playing with official server or broken file.
------------
### Login with your username then password with random then login.
### Command GM_Handbook 3.0  [Clike link](https://raw.githubusercontent.com/NPC7FULL/Genshin-impact-Join-Private-Server/main/command/GM_Handbook_-_EN.txt "Clike link")
### Command GM_Handbook 2.8  [Clike link](https://github.com/NPC7FULL/Genshin-impact-Join-Private-Server/blob/main/command/GM_Handbook%202.8.txt "Clike link")
### Command GM_Handbook 2.7  [Clike link](https://github.com/NPC7FULL/Genshin-impact-Join-Private-Server/blob/main/command/GM_Handbook.txt "Clike link")
