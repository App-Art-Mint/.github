# Sunder Apps Environment Setup
## Prepare Environment
### macOS X+ - install Homebrew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Windows 10+ - set execution policy
```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

## Install dependencies
### homebrew
```bash
brew install git gh node \
&& brew install --cask visual-studio-code
```

### winget
```powershell
winget install git.git; `
winget install github.cli; `
winget install openjs.nodejs.lts; `
winget install microsoft.visualstudiocode
```

### pacman
```bash
sudo pacman -Sy git github-cli nodejs-lts-gallium code
```

## Install angular cli globally (choose newest LTS)
```bash
npm i -g @angular/cli@14.2.10
```

## Set your git config
```bash
git config --global user.email '[email]' \
&& git config --global user.name '[name]' \
&& git config --global init.defaultBranch 'prod'
```

## Log in to GitHub CLI and follow the prompts
```bash
gh auth login
```

## Log in to npm and follow the prompts
```bash
npm adduser
```
