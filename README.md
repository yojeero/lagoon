<img src="preview/lagoon.png">

### Install Lagoon theme in Windows Terminal

- Install Fonts from folder.
- Run Windows Terminal.
- Select Settings from the Windows Terminal drop-down menu while holding the SHIFT key to open the "settings.json" file in your default text editor.
- Edit > settings.json.
- Copy all from local settings.json and insert in setting.json between the lines like this:

```json

"schemes": 
    [
        {
            "name": "Lagoon",
            "black": "#013a63",
            "red": "#ffbc42",
            "green": "#34a0a4",
            "yellow": "#fcbf49",
            "blue": "#00509d",
            "purple": "#8e7dbe",
            "cyan": "#118ab2",
            "white": "#99c1de",
            "brightBlack": "#214462",
            "brightRed": "#ffd23f",
            "brightGreen": "#aecab8",
            "brightYellow": "#ffd166",
            "brightBlue": "#014f86",
            "brightPurple": "#ada7c9",
            "brightCyan": "#61a5c2",
            "brightWhite": "#bcd4e6",
            "background": "#183752",
            "foreground": "#a3c6e6",
            "selectionBackground": "#e5ce5c",
            "cursorColor": "#79acd8"
            }
    ],

```

- Save
- Open Settings in Windows Terminal and select Lagoon theme by default theme.

Enjoy !

```
In setting.json you can change some parametres like transparent.
```

#### Theme based by MonoLisa Font for Coders [website](https://www.monolisa.dev/).

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

### OhMyPosh install in Windows Terminal

winget install JanDeDobbeleer.OhMyPosh -s winget

### Install [Nerd fonts](https://www.nerdfonts.com/font-downloads)

My favorites - Hack Nerd Font Mono or JetBrains Mono.

Select - **jandedobbeleer.omp.json** theme for OhMyPosh

oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\jandedobbeleer.omp.json" | Invoke-Expression

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

### PowerShell install

https://learn.microsoft.com/ru-ru/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.4#install-powershell-using-winget-recommended

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

```
Inside themes folder you find some of my favorite themes.
```   

### OhMyPosh Installation Guide for Windows 11 PowerShell

```   
If you see an error about execution policy, run this command in PowerShell as Administrator:
```

Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser 

##### check the current execution policy with:
Get-ExecutionPolicy -List


##### Step 1: Create the $PROFILE file if it does not exist

$PROFILE 

##### Step 2: Install OhMyPosh using Winget, Scoop, or PowerShell

#### If you use Winget, just run:

winget install JanDeDobbeleer.OhMyPosh -s winget

#### If you prefer Scoop, the command is:

scoop install https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/oh-my-posh.json

#### if you like working with PowerShell, execute:

Set-ExecutionPolicy Bypass -Scope Process -Force; Invoke-Expression ((New-Object System.Net.WebClient).DownloadString('https://ohmyposh.dev/install.ps1'))

##### Step 3: Add OhMyPosh to the PowerShell profile

#### Open the Microsoft.PowerShell_profile.ps1 file and add the following line:

oh-my-posh init pwsh | Invoke-Expression

Now, you can save and close the file.