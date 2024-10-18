### Command List 

Oi supports the following basic commands.  
###  Oi
`oi` is the entry point for the CLI application. You can use it with or without the -h flag to see the list of commands. 
### Oi init
This initialises an directory as a project, it helps oi understand which sub-directories and files needs to be watched for prompts.

**Supported Flags**
- `-i` or `--ignore` is used for adding single or multiple files to the ignore list. Files inside ignore list won't be watched for prompts and `oi` will also ignore any context they might add. 
- `-n` or `--project-name` is used to define a custom name for the project in the `oi-config.json`
- `-v` or `--verbose` this is used for capturing logs.

### Oi config
This allows the user to update the local and global config files. This can be used for adding ignore files, update project name in local config. It also has options to update the global config file.

**Supported Flags**
- `-i` or `--ignore` is used for adding single or multiple files to the ignore list. Files inside ignore list won't be watched for prompts and `oi` will also ignore any context they might add. 
- `-n` or `--project-name` is used to define a custom name for the project in the `oi-config.json`
- `-g` or `--global` is used to select a LLM | Platform to be used for getting responses to prompts. It shows the list of currently supported platform and allow user to feed required information.
- `-sa` or `--set-active` is used to switch between platforms if multiple platforms are added to the global config file. 

### Oi start
This starts the oi cli inside a directory and allows the user to generate code. It only supports one flag which is `-v` or `--verbose`.