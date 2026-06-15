## [Oh-My-Posh](https://ohmyposh.dev) Theme

### Theme colors  
`dusk_dawn`

<img width="1146" height="438" alt="image" src="https://github.com/user-attachments/assets/b00c4f3e-9aa4-4877-98c3-e8aad6d69b4c" />  

`coffee_latte`

<img width="1146" height="153" alt="image" src="https://github.com/user-attachments/assets/e84922e9-d3f0-4f3b-afca-dd6a92f509f7" />  

`berries_cream`

<img width="1146" height="153" alt="image" src="https://github.com/user-attachments/assets/8fe9bc87-123a-4abe-9024-41266b7b7672" />  

`lavender_rose`

<img width="1146" height="153" alt="image" src="https://github.com/user-attachments/assets/f7fbb5b9-2780-4064-bcf7-271e115456a3" />  

### Steps  

1. Install `Oh-My-Posh`.
``` pwsh
winget install JanDeDobbeleer.OhMyPosh --source winget
```

2. Open `Microsoft.PowerShell_profile.ps1` file.
``` pwsh
notepad $PROFILE
```

3. Paste script below & save.
``` pwsh
$themeGit = "https://raw.githubusercontent.com/bearoxo/Oh-My-Posh-Theme/refs/heads/main/aera.omp.json"
$themepPath = "C:\TEMP\aera.omp.json"

if (-not (Test-Path -Path $themePath)) { 
  curl $themeGit > $themePath
}
   
oh-my-posh init pwsh --config $themePath | Invoke-Expression

clear
```

4. Open `.omp.json` theme file.
``` pwsh
notepad $ThemePath
```

5. Change the theme color to one of the color palette presets.
``` json
"palettes": {
  "template": "dusk_dawn"
}
```
