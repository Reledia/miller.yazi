# miller.yazi

[Miller](https://github.com/johnkerl/miller) now in [yazi](https://github.com/sxyazi/yazi). To install clone the repo inside `~config/yazi/miller_csv.yazi/` and add this to your `~/.config/yazi`:

```toml
append_previewers = [
    { mime = "text/csv", exec = "miller_csv"},
]
```

To change colors of keys and values, edit the `init.lua` file after the `--key-color` and `--value-color` flags. To view a list of possible colors, use `mlr --list-color-names`. Make sure to have miller installed and inside your PATH.
