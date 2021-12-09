# Use Terminal Windows similar Linux

If you have Windows 11 you can the new terminal, but if you still have Windows 10 you need to download Windows Terminal from Microsoft Store and download Powershell

After that you need to configure your terminal with powershell.

Its necesary downlaod a new Font, can be from NerdFonds, I recommender (Hack)[https://github.com/ryanoasis/nerd-fonts/releases/tag/v2.1.0], this font works with the icons perfectly. 

## Scoop

You need to install scoope, this is a tool to install packages.
```
iwr -useb get.scoop.sh | iex
```
When you have already installed scoop you need to install curl
```
scoop curl sudo jq
```

I download Git
```
winget install -e --id Git.Git
```

And I install NeoVim that I have a explain about this in my repository (nvim)[https://github.com/Eduardo-Guerra-Alvarez/nvim]

- You need to create a file `.config/powershell/user_profile.ps1`
or download the file in my repository

and you need to edit `$PROFILE.CurrentUserCurrentHost` and into the file write down `. $env:USERPROFILE\.config\powershell\user_profile.ps1`

- To install oh-my-posh you need to write the following command:
```
Install-Module posh-git -Scope CurrentUser -Force
Install-Module oh-my-posh -Scope CurrentUser -Force
```

- To show icons in your terminal
```
Install-Module -Name Terminal-Icons -Repository PSGallery -Force
```

- To install ReadLine is a power tool very useful, show suggestions
```
Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck
```

- Fzf is a tool very useful, to search files or directorys
```
scoop isntall fzf
```


# Credits 
User devasfile from his video
[How to set up PowerShell prompt with Oh My Posh on Windows 11](https://www.youtube.com/watch?v=5-aK2_WwrmM)
