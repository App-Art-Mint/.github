# App Art Mint New App Process
## Before you begin
 - [Configure your environment](https://github.com/App-Art-Mint/.github/blob/prod/docs/prepare-env.md)

### Enter your projects directory
```bash
cd [path/to/code]
```

### Clone the workspace
```bash
gh repo clone App-Art-Mint/ngx-projects && cd ngx-projects && npm i
```

## Creating a new project
Run the following commands from the root of the workspace or in the projects folder.

### Apps
```bash
ng g application [project] --routing true --style scss && cd [project] && gh repo create App-Art-Mint/[project] --private --source=. --remote=upstream && git push && npm i
```

### Libraries
```bash
ng g library [project] && cd [project] && gh repo create App-Art-Mint/ngx-[project] --public --source=. --remote=upstream && git push && npm i
```

# Next steps:
