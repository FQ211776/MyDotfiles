# My Ultimate PowerShell prompt with starship and the Windows Terminal

**Description :**   Deleting the .git folder may cause problems in your git repository. If you want to delete all your commit history but keep the code in its current state, it is very safe to do it as in the following:

**Example** :

```powershell
# install scoop
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
iwr -useb get.scoop.sh | iex

# optional buckets
scoop bucket add extras
scoop bucket add java

# install git
scoop install git
git config --global credential.helper manager-core

# install Nerd Fonts
scoop bucket add nerd-fonts
scoop install JetBrainsMono-NF-Mono
scoop install JetBrainsMono-NF
scoop install Meslo-NF-Mono.json
scoop install Meslo-NF.json

# install sudo to elevate privileges when needed
scoop install sudo

# install windows terminal
scoop install windows-terminal
scoop install extras/vcredist2022

# install latest version of Powershell
iex "& { $(irm https://aka.ms/install-powershell.ps1) } -UseMSI"

# install starship as a default prompt
scoop install starship

# install oh-my-posh as a alternative prompt
scoop install nuget
scoop install winget
winget install oh-my-posh
install-Module posh-git  -Scope CurrentUser -Force
# install-Module oh-my-posh -Scope CurrentUser -Force
cd ~\AppData\Local
git clone https://github.com/JanDeDobbeleer/oh-my-posh.git

# Install Fzf - Fuzzy finder
scoop install fzf
Install-Module -Name PSFzf -Scope CurrentUser -ForceInstall-Module -Name PSFzf -Scope CurrentUser -Force


#  Install z - Directory jumper
sudo Install-Module -Name z -Force -AllowClobber

# Terminal Icons
sudo Install-Module -Name Terminal-Icons -Repository PSGallery -Force

# Install PSReadLine - Autocompletion
Install-Module -Name PowerShellGet -Force
sudo Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force  -SkipPublisherCheck
Set-PSReadLineOption -PredictionSource History
Set-PSReadLineOption -PredictionViewStyle listView
```


**Now lets change some settings**

![](20220427225824.png)
![](20220427225907.png)
![](20220428000303.png)

**utility command - `ctrl + r`**
![](20220427230323.png)
**utility command - `ctrl + b`**
![](20220427230249.png)
 **utility command - `which`**
![](20220427230219.png)





**showcase**
![](20220427233007.png)
![](20220427233644.png)
![](20220427234220.png)
![](20220427234632.png)


**how to set a theme**
```powershell
set-PoshPrompt M365Princess
set-PoshPrompt agnoster
set-PoshPrompt agnosterplus
set-PoshPrompt aliens
set-PoshPrompt amro
set-PoshPrompt atomic
set-PoshPrompt atomicBit
set-PoshPrompt avit
set-PoshPrompt blue-owl
set-PoshPrompt blueish
set-PoshPrompt bubbles
set-PoshPrompt bubblesextra
set-PoshPrompt bubblesline
set-PoshPrompt capr4n
set-PoshPrompt cert
set-PoshPrompt cinnamon
set-PoshPrompt clean-detailed
set-PoshPrompt cloud-native-azure
set-PoshPrompt craver
set-PoshPrompt darkblood
set-PoshPrompt default
set-PoshPrompt di4am0nd
set-PoshPrompt dracula
set-PoshPrompt emodipt
set-PoshPrompt festivetech
set-PoshPrompt fish
set-PoshPrompt free-ukraine
set-PoshPrompt gmay
set-PoshPrompt grandpa-style
set-PoshPrompt half-life
set-PoshPrompt honukai
set-PoshPrompt hotstick.minimal
set-PoshPrompt hunk
set-PoshPrompt huvix
set-PoshPrompt if_tea
set-PoshPrompt iterm2
set-PoshPrompt jandedobbeleer
set-PoshPrompt jblab_2021
set-PoshPrompt jonnychipz
set-PoshPrompt jtracey93
set-PoshPrompt jv_sitecorian
set-PoshPrompt kali
set-PoshPrompt lambda
set-PoshPrompt lambdageneration
set-PoshPrompt larserikfinholt
set-PoshPrompt M365Princess
set-PoshPrompt marcduiker
set-PoshPrompt markbull
set-PoshPrompt material
set-PoshPrompt microverse-power
set-PoshPrompt mojada
set-PoshPrompt montys
set-PoshPrompt mt
set-PoshPrompt negligible
set-PoshPrompt night-owl
set-PoshPrompt nordtron
set-PoshPrompt nu4a
set-PoshPrompt paradox
set-PoshPrompt pararussel
set-PoshPrompt patriksvensson
set-PoshPrompt peru
set-PoshPrompt pixelrobots
set-PoshPrompt plague
set-PoshPrompt powerlevel10k_classic
set-PoshPrompt powerlevel10k_lean
set-PoshPrompt powerlevel10k_modern
set-PoshPrompt powerlevel10k_rainbow
set-PoshPrompt powerline
set-PoshPrompt probua.minimal
set-PoshPrompt pure
set-PoshPrompt remk
set-PoshPrompt robbyrussel
set-PoshPrompt rudolfs-dark
set-PoshPrompt rudolfs-light
set-PoshPrompt schema.json
set-PoshPrompt slim
set-PoshPrompt slimfat
set-PoshPrompt smoothie
set-PoshPrompt sonicboom_dark
set-PoshPrompt sonicboom_light
set-PoshPrompt sorin
set-PoshPrompt space
set-PoshPrompt spaceship
set-PoshPrompt star
set-PoshPrompt stelbent.minimal
set-PoshPrompt takuya
set-PoshPrompt the-unnamed
set-PoshPrompt thecyberden
set-PoshPrompt tiwahu
set-PoshPrompt tonybaloney
set-PoshPrompt unicorn
set-PoshPrompt velvet
set-PoshPrompt wopian
set-PoshPrompt xtoys
set-PoshPrompt ys
set-PoshPrompt zash
```

