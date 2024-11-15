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
brew install git gh nvm awscli \
&& brew install --cask visual-studio-code
```

### winget
(NOTE: If you don't have winget, install Package Installer from the Microsoft Store and reboot)
```powershell
winget install git.git; `
winget install github.cli; `
winget install coreybutler.nvmforwindows; `
winget install amazon.awscli; `
winget install microsoft.visualstudiocode
```

## Install Node
```bash
nvm install 20.18.0
nvm use 20.18.0
```

## Install global CLI tools
NOTE: On MacOS and Linux, you may need to run this command with sudo

```bash
npm i -g @angular/cli cordova aws-cdk
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

## Set up SSO for AWS CLI
Follow the prompts to set up SSO for your profile.
(First Prompt:) Set a unique SSO session name.
(Final Prompt:) Ensure that the profile name matches the profile name in the package.json of the project you are working on.
```bash
aws configure sso
```

## Sign in to AWS CLI as needed
```bash
aws sso login --profile [profile-name]
```
