# webc-vscode

Language tooling for [11ty WebC components](https://www.11ty.dev/docs/languages/webc/) built using the [Volar framework](https://volarjs.dev/).

> [!WARNING]
> _This is extremely extremely new and very incomplete tooling. Proceed with caution._

## Features

- Basic syntax highlighting for HTML, CSS, JavaScript, and YAML-based frontmatter
- Embedded language services for HTML, CSS, and JavaScript
  - Completions
  - Emmet support
  - Language-specific diagnostics

## Try `webc-vscode` on your local machine

- Run `pnpm install` in the root directory
- Run `pnpm run pack` in this folder
- A `vscode-webc-0.0.1.vsix` file will be created at `packages/vscode/`
- Open the VS Code command palette and run `Extensions: Install from VSIX...`
- Select the `.vsix` file that was just generated
- You've installed the extension and can try it out in a WebC project!

## Development: Running the sample

- Run `pnpm install` in the root directory
- Open VS Code from the root folder
- Press `Ctrl+Shift+B` (or `Cmd+Shift+B`) to compile the client and server
- Switch to the "Run and Debug" view
- Select `Launch Client` from the dropdown
- Run the launch config
- If you want to debug the server as well use the launch configuration `Attach to Server`
- In the [Extension Development Host] instance of VSCode, open the `test1.webc` and `test2.webc` files
  - Type `<d` to try HTML completion
  - Type `<style>.foo { c }</style>` to try CSS completion
  - Have `<style>.foo { }</style>` to see CSS Diagnostics

## Development: References

- https://code.visualstudio.com/api/language-extensions/embedded-languages
- https://github.com/microsoft/vscode-extension-samples/tree/main/lsp-embedded-language-service
