# App Art Mint New App Process
## Before you begin
 - [Configure your environment](https://github.com/App-Art-Mint/.github/blob/prod/docs/prepare-env.md)

### Enter your projects directory
```bash
cd [path/to/code]
```

## Creating a new project
Run the following commands from the root of the workspace or in the projects folder.

### Apps
```bash
ng new [project] --routing true --style scss && cd [project] && gh repo create App-Art-Mint/[project] --private --source=. && git push && npm i
```
