# App Art Mint Environment Setup
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
(NOTE: Replace Node with nvm)
### homebrew
```bash
brew install git gh nvm \
&& brew install --cask visual-studio-code
```

### winget
(NOTE: If you don't have winget, install Package Installer from the Microsoft Store and reboot)
```powershell
winget install git.git; `
winget install github.cli; `
winget install coreybutler.nvmforwindows; `
winget install microsoft.visualstudiocode
```

## Install Node
```bash
nvm install lts
```

## Install global CLI tools
NOTE: On MacOS and Linux, you may need to run this command with sudo

```bash
npm i -g @angular/cli@latest cordova@latest @aws-amplify/cli@latest
```

## Set your git config
```bash
git config --global user.email '[email]' \
&& git config --global user.name '[name]' \
&& git config --global init.defaultBranch 'prod' \
&& git config --global push.autoSetupRemote true
```

## Log in to GitHub CLI and follow the prompts
```bash
gh auth login
```

## Log in to npm and follow the prompts
```bash
npm login
```

## Log in to AWS Amplify and follow the prompts
```bash
amplify configure
```
