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
ng new [project] --routing true --style scss --ssr false
```

#### Create a Next application
```bash
npx create-next-app@latest [project] --ts --eslint --no-tailwind --app --src-dir --turbopack --import-alias "@/*" --react-compiler
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

### Configure Template

#### Any project
##### Copy .npmrc, amplify.yml, .env, tsconfig.json
##### Update tsconfig with paths && noPropertyAccessFromIndexSignature
##### Copy tinify script
##### Update package.json scripts
##### Add global styles

#### Angular project
##### Copy polyfills
##### Copy environment.ts
##### Update .editorconfig
##### angular.json Updates
###### Styles
###### Assets
###### Output Path
###### Preserve Symlinks
###### Output Hashing
###### Budgets



### Install dependencies

#### Any project
```bash
npm i @appartmint/css-mint @appartmint/ts-mint photoswipe swiper tinify square papaparse pngjs probe-image-size
```
```bash
npm i -D @aws-sdk/client-cognito-identity-provider @types/aws-lambda madge @types/papaparse @types/pngjs @types/probe-image-size @types/grecaptcha npm-run-all2 cross-replace @dotenvx/dotenvx sass
```

#### Angular project
```bash
npm i @angular/material @aws-amplify/ui-angular
```

#### Next project
```bash
npm i 
```

### Configure AWS Account
- Create AWS Account in AWS Organizations
- Move AWS Account to workloads folder in AWS Organizations
- In IAM Identity Center, assign admin access to the user
- Configure SSO
```bash
aws configure sso
```
- First name: [user]-[host]-[account]
e.g. sunder-sbox-app-art-mint
- Profile name: [account]
e.g. app-art-mint


### Configure Amplify
#### Set secrets (add to sandbox too)
#### Set Node 20 LTS
#### Create dev branch
#### Configure previews

