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

### Copy .npmrc, amplify.yml, .env
### Copy polyfills
### Copy environment.ts
### Copy tinify script
### Update package.json scripts
### Update .editorconfig
### Update tsconfig with paths && noPropertyAccessFromIndexSignature
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
npm i @appartmint/mint @appartmint/util @angular/material @aws-amplify/ui-angular photoswipe swiper tinify square papaparse pngjs probe-image-size @dotenvx/dotenvx
```

```bash
npm i -D @aws-sdk/client-cognito-identity-provider @types/aws-lambda madge @types/papaparse @types/pngjs @types/probe-image-size npm-run-all2 cross-replace
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




## Configure backend separately
```bash
npm i @dotenvx/dotenvx
```



npm r npm-run-all
npm i -D npm-run-all2

replace npm-run-all with run-s
delete upgrade scripts
v19

.npmrc

npm run update
npm run login
npm run use:sandbox
npm run gen:graphql

npm run serve


.env