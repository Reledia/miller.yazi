# miller.yazi

[Miller](https://github.com/johnkerl/miller) now in [yazi](https://github.com/sxyazi/yazi). To install clone the version you want (csv and/or json) inside `~config/yazi/miller_csv.yazi/` or `~/.config/yazi/miller_json.yazi/` and add this to your `~/.config/yazi`:

```toml
append_previewers = [
    { mime = "text/csv", exec = "miller_csv"},
    { mime = "application/json", exec = "miller_json"},
]
```

To change colors of keys and values, edit the `init.lua` file after the `--key-color` and `--value-color` flags. To view a list of possible colors, use `mlr --list-color-names`. Make sure to have miller installed and inside your PATH.
