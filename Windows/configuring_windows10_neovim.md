# Neovim in Windows 10

**Description :**

## PowerShell setup (Windows)

- [Scoop](https://scoop.sh/) - A command-line installer
- [Git for Windows](https://gitforwindows.org/)
- [Oh My Posh](https://ohmyposh.dev/) - Prompt theme engine
- [Terminal Icons](https://github.com/devblackops/Terminal-Icons) - Folder and file icons
- [PSReadLine](https://docs.microsoft.com/en-us/powershell/module/psreadline/) - Cmdlets for customizing the editing environment, used for autocompletion
- [z](https://www.powershellgallery.com/packages/z) - Directory jumper
- [PSFzf](https://github.com/kelleyma49/PSFzf) - Fuzzy finder

**Example** :

```powershell
# install neovim and tools needed
scoop install neovim
scoop install gcc
scoop install mingw

# Neovim GUI <optional>
scoop install goneovim
scoop install neovim-qt
scoop install fvim

# install NVChad
git clone https://github.com/wbthomason/packer.nvim $env:LOCALAPPDATA\nvim-data\site\pack\packer\start\packer.nvim
git clone https://github.com/wbthomason/packer.nvim "$env:LOCALAPPDATA\nvim-data\site\pack\packer\start\packer.nvim"
git clone https://github.com/NvChad/NvChad nvim --depth 1
#Copy the nvim dir to ~/AppData/Local/ and then
nvim +'hi NormalFloat guibg=#1e222a' +PackerSync

# install VIFM
scoop install vifm

# remember to copy this folders in order to get favicom icons in vifm
# .config
# .vifm
# favicons.vifm
```


**showcase**
![](20220428112801.png)
![](20220428112543.png)
