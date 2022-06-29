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
curl   --output %USERPROFILE%\Desktop\Genshin_Private_Server\setup

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
### Login with your username then password with random then login.
#### Command GM_Handbook  [Clike link](https://github.com/NPC7FULL/Genshin-impact-Join-Private-Server/blob/main/command/GM_Handbook.txt "Clike link")
