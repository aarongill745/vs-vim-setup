# vs-vim-setup

## General
* Move primary sidebar to the right
* Get rid of minimap
* Install favourite theme

## Update keybindings.json:
```json
// Place your key bindings in this file to override the defaults
[
    {
        "key": "tab",
        "command": "tab",
        "when": "editorTextFocus && !editorTabMovesFocus"
    },
    {
        "key": "shift+tab",
        "command": "outdent",
        "when": "editorTextFocus && !editorTabMovesFocus"
    },
]
```

## Update settings.json:
```json 
{
    "workbench.sideBar.location": "right",
    "vim.insertModeKeyBindings": [
        {
            "before": [
                "k", "j"
            ],
            "after": ["<Esc>"]
        },
    ],
    "editor.minimap.enabled": false,
    "vim.handleKeys": {
            "<C-p>": false
    },
    "vim.useCtrlKeys": false
}
```

## Update settings
Line Number: on --> relative

