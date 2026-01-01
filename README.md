# Zed PureScript

A [PureScript](https://www.purescript.org/) extension for [Zed](https://zed.dev).

## Configuration

### Environment Variables

You can specify arguments as well as environment variables to pass to the language server by configuring the `lsp` settings in your Zed settings. This can be helpful for Nix setups or other environments where you need to customize the `PATH` or other variables so that the language server can find the purescript binary to invoke for the LSP support.

Example configuration in your `settings.json`:

```json
{
    "lsp": {
        "purescript-language-server": {
            "binary": {
                "env": {
                    "PATH": "/nix/store/gw58kr741a9ddmv3xn47llc7i07jbbvr-purescript-0.15.15/bin"
                }
            }
        }
    }
}
```

## Development

To develop this extension, see the [Developing Extensions](https://zed.dev/docs/extensions/developing-extensions) section of the Zed docs.
