# Unix

Export all installed extensions to a file **code_installed_extension.txt**
```bash
code --list-extensions | xargs -L 1 echo code --install-extension > code_installed_extension.txt
```

Import all saved packages from file **code_installed_extension.txt**
```bash
sh ./code_installed_extension.txt
```

# Window - PowerShell
```bash
code --list-extensions | % { "code --install-extension $_" }
```

# Command
```bash
code --help
code --version
code --list-extensions
code --install-extension ext-name

# --list-extensions-json
# --list-extensions-enabled
# --list-extensions-disabled
# --install-extensions-json
# --install-extension-disabled
```

# Path
```bash
Windows: %USERPROFILE%\.vscode\extensions
Mac: ~/.vscode/extensions
Linux: ~/.vscode/extensions
```

https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync
