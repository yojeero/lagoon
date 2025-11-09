<img src="preview/lagoon.png">

#### Install Lagoon theme in Windows Terminal

1. Install Fonts from folder.
2. Run Windows Terminal.
3. Select Settings from the Windows Terminal drop-down menu while holding the SHIFT key to open the "settings.json" file in your default text editor.
4. Edit > settings.json.
5. Copy all from local settings.json and insert in setting.json between the lines like this:
6. Save the file and restart Windows Terminal.

#### OhMyPosh install in Windows Terminal

winget install JanDeDobbeleer.OhMyPosh

new-item -type file -path $profile -force

notepad $PROFILE

```
save file and restart terminal. If the theme is not applied, run the following command in PowerShell:
```

. $PROFILE

oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\jandedobbeleer.omp.json" | Invoke-Expression

```   
Add OhMyPosh to the PowerShell profile
```

oh-my-posh init pwsh | Invoke-Expression 

```      
If you see an error about execution policy, run this command in PowerShell:

Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser 
```