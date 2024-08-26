# App Art Mint New App Process
## Before you begin
 - [Configure your environment](https://github.com/App-Art-Mint/.github/blob/prod/docs/prepare-env.md)

### Enter your projects directory
```bash
cd [path/to/code]
```

## Creating a new project
Run the following commands from the root of the workspace or in the projects folder.

### Create an Angular application
```bash
ng new [project] --routing true --style scss --no-standalone --ssr false
```

### Enter the app's directory
```bash
cd [project]
```

### Create a GitHub repo
```bash
gh repo create App-Art-Mint/[project] --private --source=. && git push
```

### Add Amplify
```bash
npm create amplify@latest
```

### Copy .npmrc and polyfills
### Copy amplify.yml (update out dir)
### Update package.json scripts
### Update .editorconfig
### Update tsconfig with paths && noPropertyAccessFromIndexSignature
### Update tsconfig.app with mint
### Add global styles
### Angular Updates
#### Styles
#### Assets
#### Output Path
#### Preserve Symlinks
#### Output Hashing
#### Budgets



### Install dependencies
```bash
npm i @appartmint/mint @appartmint/util @aws-amplify/ui-angular "@awesome.me/kit-c0365045dc" photoswipe swiper
```

### Configure Amplify
#### Set secrets (add to sandbox too)
#### Set Node 20.13.1
#### Create dev branch
#### Configure previews