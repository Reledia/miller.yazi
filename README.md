# miller.yazi

[Miller](https://github.com/johnkerl/miller) now in [yazi](https://github.com/sxyazi/yazi). To install, clone the repo inside `~/.config/yazi/plugins/`:

```toml
[plugin]
prepend_previewers = [
    { mime = "text/csv", run = "miller"},
]
```

## Preview

![preview](https://github.com/Reledia/miller.yazi/blob/main/preview.png?raw=true)

## Color

To change colors of keys and values, edit the `init.lua` file after the `--key-color` and `--value-color` flags. To view a list of possible colors, use `mlr --list-color-names`. Make sure to have miller installed and inside your PATH.

## Other types of file

To adapt this plugin to the other format supported from miller (like json):
- copy the plugin folder
- change the name of the copied folder into miller_(fmt)
- change the `--icsv` flag inside `init.lua` to `--i(fmt)`
- add the correct mime/name rule into `prepend_previewers` and the exec as `miller_(fmt)`
