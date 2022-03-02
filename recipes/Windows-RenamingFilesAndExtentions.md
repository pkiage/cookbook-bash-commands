# Renaming Files and Extentions

## Add perfix to file names
### Generic: Command Prompt
```bash
for %i in (*.*) do ren "%i" "<prefix>%i"
```

### Example: Command Prompt: Add prefix "Review-" to filenames
```bash
for %i in (*.*) do ren "%i" "Review-%i"
```

## Remove perfix from file names

### Example: Remove "Review-" from mp4 files
```bash
rename "Review-*.mp4" "///////*.mp4"
```

> *The number of backslashes should be the same as number of characters being removed 
 e.g. "Review-" has 7 characters therefore using 7 backslashes.*  

### Example: PowerShell: Remove the first 7 characters from mp4 files

```bash
Get-ChildItem *.mp4 | Rename-Item -NewName {[String]($_.Name).Substring(7)}
```

## Add suffix to file names


## Remove suffix from file names
### Example: PowerShell: Remove the last 3 characters from mp4 files
```bash
Get-ChildItem *.mp4 | Rename-Item -NewName {$_.Name.Substring(0,$_.BaseName.Length-3) + $_.Extension -Replace “_”,” “}
```

### Example: PowerShell: Remove the last 4 characters from jpg files
```bash
Get-ChildItem *.jpg | Rename-Item -NewName {$_.Name.Substring(0,$_.BaseName.Length-4) + $_.Extension -Replace “_”,” “}
```

## Change extension
### Generic
```bash
ren *.<initial_extention> *.<new_extention>
```

### Example: Change extension from .bin to .mp4
```bash
ren *.bin *.mp4
```

# References and Guides

https://docs.microsoft.com/en-us/powershell/scripting/learn/ps101/02-help-system?view=powershell-7.2

https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/help

https://www.gnu.org/prep/standards/html_node/_002d_002dhelp.html#g_t_002d_002dhelp

https://www.gnu.org/software/guile/manual/html_node/Help-Commands.html

https://ss64.com/
