# My Sublime Text Setup

## User Settings

```json
{
    "font_size": 12,
    "translate_tabs_to_spaces": true,
    "shift_tab_unindent": true,
    "auto_find_in_selection": true,
    "highlight_modified_tabs": true,
    "hot_exit": "disabled",
    
    "ignored_packages":
    [
        "Vintage",
     ],
}
```

## Packages
 - Terminus
 - GitGutter
 - AutoDocString
 - LSP
 - LSP-json
 - LSP-pylsp
 - LSP-pyright

## Package Settings

### Terminus
#### Settings
```json
{
    "256color": true,
    "unix_term": "xterm-256color",
    "unix_lang": "en_GB.UTF-8",
}
```

#### Command Palette
```json
[
   {
        "caption": "Terminal (panel)",
        "command": "terminus_open",
        "args"   : {
           "cmd": "bash",
           "cwd": "${file_path:${folder}}",
           "title": "Command Prompt",
           "panel_name": "Terminus"
        }
   },
] 
```

#### Keybindings
```json
[
   {
       "keys": ["alt+1"],
       "command": "terminus_open",
       "args" : {
           "cmd": "bash",
           "cwd": "${file_path:${folder}}",
           "panel_name": "Terminus"
       }
   }
] 
```

### LSP-pylsp
#### Settings
```json
{
    "disabled_capabilities": {
        "completionProvider": true,
        "definitionProvider": true,
        "documentHighlightProvider": true,
        "documentSymbolProvider": true,
        "hoverProvider": true,
        "referencesProvider": true,
        "renameProvider": true,
        "signatureHelpProvider": true,
    },
    "settings": {
        "pylsp.plugins.jedi_completion.enabled": false,
        "pylsp.plugins.jedi_definition.enabled": false,
        "pylsp.plugins.jedi_hover.enabled": false,
        "pylsp.plugins.jedi_references.enabled": false,
        "pylsp.plugins.jedi_signature_help.enabled": false,
        "pylsp.plugins.jedi_symbols.enabled": false,
    },
}
```

