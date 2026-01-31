# Helpful Terminal Commands

## PowerShell

### For each folder, run...
```bash
$array = @("folder1", "folder2"); $array | ForEach-Object { Invoke-Expression "cd ../$_; npm run update:mint" }
```
