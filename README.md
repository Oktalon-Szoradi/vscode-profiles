# vscode-profiles

## In a nutshell:

### Oktalon
My personal VS Code profile for personal projects. Has the most extensions, and forces an opiniated JavaScript style ([StandardJS](https://standardjs.com/)).

### SchoolPLF
Lite profile for PLFs (praktische Leistungsfeststellungen (practical performance assessments)) at school.  
Has extensions required for fullstack development that uses ESLint, Vue, Vitest.

## Specifics:

### SchoolPLF

#### Settings:

```json
{
  "[javascript]": {
    "editor.defaultFormatter": "dbaeumer.vscode-eslint"
  },
  "[vue]": {
    "editor.defaultFormatter": "Wscats.vue"
  },
  "dotenv.enableAutocloaking": false,
  "editor.cursorBlinking": "phase",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.fontFamily": "'Fira Code', 'monospace', monospace",
  "editor.fontLigatures": true,
  "editor.formatOnSave": true,
  "editor.guides.bracketPairs": true,
  "editor.inlineSuggest.enabled": true,
  "editor.linkedEditing": true,
  "editor.mouseWheelZoom": true,
  "editor.quickSuggestions": {
    "strings": true
  },
  "editor.smoothScrolling": true,
  "editor.suggestSelection": "first",
  "editor.tabSize": 2,
  "editor.tokenColorCustomizations": {
    "textMateRules": []
  },
  "editor.wordWrap": "off",
  "eslint.format.enable": true,
  "files.associations": {
    ".env*": "dotenv"
  },
  "files.autoSave": "afterDelay",
  "indentRainbow.colors": [
    "rgba(7, 142, 112, 0.1)",
    "rgba(38, 207, 170, 0.1)",
    "rgba(153, 232, 193, 0.1)",
    "rgba(255, 255, 255, 0.1)",
    "rgba(123, 173, 226, 0.1)",
    "rgba(79, 72, 203, 0.1)",
    "rgba(61, 26, 119, 0.1)",
    "rgba(79, 72, 203, 0.1)",
    "rgba(123, 173, 226, 0.1)",
    "rgba(255, 255, 255, 0.1)",
    "rgba(153, 232, 193, 0.1)",
    "rgba(38, 207, 170, 0.1)"
  ],
  "togglequotes.chars": [
    "\"",
    "'",
    "`"
  ],
  "vue3snippets.singleQuote": true,
  "workbench.iconTheme": "material-icon-theme",
  "workbench.productIconTheme": "material-product-icons"
}
```

#### Keyboard Shortcuts:

```json
// Place your key bindings in this file to override the defaultsauto[]
[
  {
    "key": "ctrl+shift+c",
    "command": "-workbench.action.terminal.openNativeConsole",
    "when": "!terminalFocus"
  },
  {
    "key": "ctrl+shift+[Semicolon]",
    "command": "workbench.action.terminal.new"
  },
  {
    "key": "ctrl+[Backslash]",
    "command": "editor.action.commentLine",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+shift+7",
    "command": "-editor.action.commentLine",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+k ctrl+[Backslash]",
    "command": "editor.foldAllBlockComments",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+k ctrl+shift+7",
    "command": "-editor.foldAllBlockComments",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+[Quote]",
    "command": "editor.togglequotes"
  },
  {
    "key": "ctrl+shift+[Backslash]",
    "command": "-editor.togglequotes"
  },
  {
    "key": "ctrl+shift+[Backslash]",
    "command": "editor.action.blockComment",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+shift+a",
    "command": "-editor.action.blockComment",
    "when": "editorTextFocus && !editorReadonly"
  }
]
```

#### Extensions:

- Better Comments (aaron-bond.better-comments)
- undefined (bradgashler.htmltagwrap)
- Auto Import (steoates.autoimport)
- Dotenv Official +Vault (dotenv.dotenv-vscode)
- ESLint (dbaeumer.vscode-eslint)
- Error Lens (usernamehw.errorlens)
- Import Cost (wix.vscode-import-cost)
- JavaScript Booster (sburg.vscode-javascript-booster)
- Javascript Auto Backticks (chamboug.js-auto-backticks)
- Live Preview (ms-vscode.live-server)
- Live Server (Five Server) (yandeu.five-server)
- Material Icon Theme (pkief.material-icon-theme)
- Material Product Icons (pkief.material-product-icons)
- Package Json Upgrade (codeandstuff.package-json-upgrade)
- REST Client (humao.rest-client)
- SCSS Formatter (sibiraj-s.vscode-scss-formatter)
- Sass (.sass only) (syler.sass-indented)
- Sort JSON objects (richie5um2.vscode-sort-json)
- Sort package.json (unional.vscode-sort-package-json)
- Surround (sword.vscode-surround)
- Svg Preview (simonsiefke.svg-preview)
- Toggle Quotes (britesnow.vscode-toggle-quotes)
- Twoslash Query Comments (orta.vscode-twoslash-queries)
- Vitest (zixuanchen.vitest-explorer)
- Vue 3 Support - All In One (wscats.vue)
- Vue Language Features (Volar) (vue.volar)
- Vue VSCode Snippets (sdras.vue-vscode-snippets)
- eslint-disable-snippets (drknoxy.eslint-disable-snippets)
- npm Intellisense (christian-kohler.npm-intellisense)
- undefined (oderwat.indent-rainbow)
- vscode-styled-components (styled-components.vscode-styled-components)

### Oktalon

#### Settings:

```json
{
  "[bibtex]": {
    "editor.defaultFormatter": "James-Yu.latex-workshop"
  },
  "[csharp]": {
    "editor.defaultFormatter": "ms-dotnettools.csharp"
  },
  "[css]": {
    "editor.defaultFormatter": "aeschli.vscode-css-formatter"
  },
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  },
  "[javascript]": {
    "editor.defaultFormatter": "numso.prettier-standard-vscode"
  },
  "[json]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[latex]": {
    "editor.defaultFormatter": "James-Yu.latex-workshop"
  },
  "[python]": {
    "editor.formatOnType": true
  },
  "[sass]": {
    "editor.defaultFormatter": "syler.sass-indented"
  },
  "[typescript]": {
    "editor.defaultFormatter": "numso.prettier-standard-vscode"
  },
  "[vue]": {
    "editor.defaultFormatter": "Wscats.vue"
  },
  "autoimport.useSemiColon": false,
  "dotenv.enableAutocloaking": false,
  "editor.cursorBlinking": "phase",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.fontFamily": "'Fira Code', 'monospace', monospace",
  "editor.fontLigatures": true,
  "editor.formatOnSave": true,
  "editor.formatOnType": true,
  "editor.guides.bracketPairs": true,
  "editor.inlineSuggest.enabled": true,
  "editor.linkedEditing": true,
  "editor.mouseWheelZoom": true,
  "editor.quickSuggestions": {
    "strings": true
  },
  "editor.smoothScrolling": true,
  "editor.suggestSelection": "first",
  "editor.tabSize": 2,
  "editor.tokenColorCustomizations": {
    "[*Light*]": {
      "textMateRules": [
        {
          "scope": "ref.matchtext",
          "settings": {
            "foreground": "#000"
          }
        }
      ]
    },
    "[*Dark*]": {
      "textMateRules": [
        {
          "scope": "ref.matchtext",
          "settings": {
            "foreground": "#fff"
          }
        }
      ]
    },
    "textMateRules": []
  },
  "editor.wordWrap": "off",
  "emmet.showSuggestionsAsSnippets": true,
  "files.associations": {
    ".env*": "dotenv"
  },
  "files.autoSave": "afterDelay",
  "git.autofetch": true,
  "github.copilot.enable": {
    "*": true,
    "markdown": true,
    "plaintext": true,
    "scminput": false,
    "yaml": false
  },
  "html.autoClosingTags": true,
  "http.proxyAuthorization": null,
  "indentRainbow.colorOnWhiteSpaceOnly": true,
  "indentRainbow.colors": [
    "rgba(7, 142, 112, 0.1)",
    "rgba(38, 207, 170, 0.1)",
    "rgba(153, 232, 193, 0.1)",
    "rgba(255, 255, 255, 0.1)",
    "rgba(123, 173, 226, 0.1)",
    "rgba(79, 72, 203, 0.1)",
    "rgba(61, 26, 119, 0.1)",
    "rgba(79, 72, 203, 0.1)",
    "rgba(123, 173, 226, 0.1)",
    "rgba(255, 255, 255, 0.1)",
    "rgba(153, 232, 193, 0.1)",
    "rgba(38, 207, 170, 0.1)"
  ],
  "indentRainbow.excludedLanguages": [
    "COBOL",
    "COBOLIT",
    "COBOL_MF_PREP",
    "COBOL_MF_LISTFILE",
    "COBOL_ACU_LISTFILE",
    "COBOL_PCOB_LISTFILE",
    "plaintext"
  ],
  "indentRainbow.ignoreErrorLanguages": ["*", "markdown"],
  "javascript.autoClosingTags": true,
  "javascript.format.semicolons": "remove",
  "javascript.preferences.quoteStyle": "single",
  "javascript.suggest.autoImports": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "latex-workshop.bibtex-format.sort.enabled": true,
  "latex-workshop.latex.autoClean.run": "onSucceeded",
  "liveServer.settings.donotShowInfoMsg": true,
  "ltex.language": "de-AT",
  "prettier.arrowParens": "avoid",
  "prettier.bracketSpacing": true,
  "prettier.endOfLine": "auto",
  "prettier.htmlWhitespaceSensitivity": "strict",
  "prettier.jsxSingleQuote": true,
  "prettier.printWidth": 120,
  "prettier.semi": false,
  "prettier.singleQuote": true,
  "prettier.trailingComma": "none",
  "prettier.useEditorConfig": false,
  "prettier.vueIndentScriptAndStyle": true,
  "remote.SSH.configFile": "C:\\Users\\Talon-School\\.ssh\\config",
  "remote.SSH.remotePlatform": {
    "192.168.31.105": "linux",
    "192.168.45.105": "linux",
    "192.168.68.111": "linux",
    "192.168.68.121": "linux",
    "192.168.68.131": "linux",
    "192.168.93.105": "linux",
    "192.168.234.105": "linux"
  },
  "scssFormatter.singleQuote": true,
  "scssFormatter.trailingComma": "none",
  "standard.autoFixOnSave": true,
  "standard.enableGlobally": true,
  "terminal.integrated.defaultProfile.windows": "Command Prompt",
  "terminal.integrated.fontFamily": "'Fira Code', 'monospace', monospace",
  "togglequotes.chars": ["\"", "'", "`"],
  "typescript.autoClosingTags": true,
  "typescript.format.semicolons": "remove",
  "typescript.preferences.quoteStyle": "single",
  "typescript.suggest.autoImports": true,
  "typescript.updateImportsOnFileMove.enabled": "always",
  "vue3snippets.jsxSingleQuote": true,
  "vue3snippets.printWidth": 120,
  "vue3snippets.semi": false,
  "vue3snippets.singleQuote": true,
  "vue3snippets.trailingComma": "none",
  "workbench.colorTheme": "Default Light Modern",
  "workbench.editorAssociations": {
    "*.pdf": "latex-workshop-pdf-hook"
  },
  "workbench.iconTheme": "material-icon-theme",
  "workbench.list.smoothScrolling": true,
  "workbench.productIconTheme": "material-product-icons"
}
```

#### Keyboard Shortcuts:

```json
// Place your key bindings in this file to override the defaultsauto[]
[
  {
    "key": "ctrl+shift+c",
    "command": "-workbench.action.terminal.openNativeConsole",
    "when": "!terminalFocus"
  },
  {
    "key": "ctrl+shift+[Semicolon]",
    "command": "workbench.action.terminal.new"
  },
  {
    "key": "ctrl+[Backslash]",
    "command": "editor.action.commentLine",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+shift+7",
    "command": "-editor.action.commentLine",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+k ctrl+[Backslash]",
    "command": "editor.foldAllBlockComments",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+k ctrl+shift+7",
    "command": "-editor.foldAllBlockComments",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "ctrl+[Quote]",
    "command": "editor.togglequotes"
  },
  {
    "key": "ctrl+shift+[Backslash]",
    "command": "-editor.togglequotes"
  },
  {
    "key": "ctrl+shift+[Backslash]",
    "command": "editor.action.blockComment",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+shift+a",
    "command": "-editor.action.blockComment",
    "when": "editorTextFocus && !editorReadonly"
  }
]
```

#### Extensions:

- Autoprefixer (mrmlnc.vscode-autoprefixer)
- Better Comments (aaron-bond.better-comments)
- Bootstrap IntelliSense (hossaini.bootstrap-intellisense)
- C# (ms-dotnettools.csharp)
- CSS Flexbox Cheatsheet (dzhavat.css-flexbox-cheatsheet)
- CSS Formatter (aeschli.vscode-css-formatter)
- Dotenv Official +Vault (dotenv.dotenv-vscode)
- ESLint (dbaeumer.vscode-eslint)
- Format Files (jbockle.jbockle-format-files)
- GitHub Copilot (github.copilot)
- GitHub Copilot Chat (github.copilot-chat)
- GitHub Markdown Preview (bierner.github-markdown-preview)
- HTML CSS Support (ecmel.vscode-html-css)
- Headwind (heybourn.headwind)
- Inline fold (moalamri.inline-fold)
- JavaScript Docstrings (massi.javascript-docstrings)
- JavaScript standardjs styled snippets (capaj.vscode-standardjs-snippets)
- Javascript Auto Backticks (chamboug.js-auto-backticks)
- LaTeX Workshop (james-yu.latex-workshop)
- Markdown Checkboxes (bierner.markdown-checkbox)
- Markdown Emoji (bierner.markdown-emoji)
- Markdown Footnotes (bierner.markdown-footnotes)
- Markdown Preview Github Styling (bierner.markdown-preview-github-styles)
- Markdown Preview Mermaid Support (bierner.markdown-mermaid)
- Markdown yaml Preamble (bierner.markdown-yaml-preamble)
- Marp for VS Code (marp-team.marp-vscode)
- Package Json Upgrade (codeandstuff.package-json-upgrade)
- Path Intellisense (christian-kohler.path-intellisense)
- Prettier - Code formatter (esbenp.prettier-vscode)
- REST Client (humao.rest-client)
- Toggle Quotes (britesnow.vscode-toggle-quotes)
- Vue Snippets StandardJS (andersonmfjr.vue-snippets-standardjs)
- undefined (bradgashler.htmltagwrap)
- .NET Install Tool (ms-dotnettools.vscode-dotnet-runtime)
- .gitignore Generator (piotrpalarz.vscode-gitignore-generator)
- Auto Import (steoates.autoimport)
- Bootstrap Class Autocomplete (torresgol10.bootstrap-class-autocomplete)
- CSS sorter (zascal.css-sorter)
- Error Lens (usernamehw.errorlens)
- Import Cost (wix.vscode-import-cost)
- JavaScript Booster (sburg.vscode-javascript-booster)
- LTeX – LanguageTool grammar/spell checking (valentjn.vscode-ltex)
- Live Preview (ms-vscode.live-server)
- Live Server (ritwickdey.liveserver)
- Live Share (ms-vsliveshare.vsliveshare)
- Markdown All in One (yzhang.markdown-all-in-one)
- Markdown PDF (yzane.markdown-pdf)
- Markdown Preview Enhanced (shd101wyy.markdown-preview-enhanced)
- Material Icon Theme (pkief.material-icon-theme)
- Material Product Icons (pkief.material-product-icons)
- Prettier ESLint (rvest.vs-code-prettier-eslint)
- Prettier-Standard - JavaScript formatter (numso.prettier-standard-vscode)
- Rainbow CSV (mechatroner.rainbow-csv)
- Remote - SSH (ms-vscode-remote.remote-ssh)
- Remote - SSH: Editing Configuration Files (ms-vscode-remote.remote-ssh-edit)
- Remote Explorer (ms-vscode.remote-explorer)
- undefined (oderwat.indent-rainbow)
- SCSS Formatter (sibiraj-s.vscode-scss-formatter)
- SQLite Viewer (qwtel.sqlite-viewer)
- SVG (jock.svg)
- Sass (.sass only) (syler.sass-indented)
- Sort JSON objects (richie5um2.vscode-sort-json)
- Sort package.json (unional.vscode-sort-package-json)
- StandardJS - JavaScript Standard Style (standard.vscode-standard)
- Stylelint (stylelint.vscode-stylelint)
- Surround (sword.vscode-surround)
- Svg Preview (simonsiefke.svg-preview)
- Tailwind CSS IntelliSense (bradlc.vscode-tailwindcss)
- Twoslash Query Comments (orta.vscode-twoslash-queries)
- TypeScript Vue Plugin (Volar) (vue.vscode-typescript-vue-plugin)
- Vitest (zixuanchen.vitest-explorer)
- Vue 3 Support - All In One (wscats.vue)
- Vue Language Features (Volar) (vue.volar)
- Vue VSCode Snippets (sdras.vue-vscode-snippets)
- Vue Volar extension Pack (misterj.vue-volar-extention-pack)
- colorize (kamikillerto.vscode-colorize)
- eslint-disable-snippets (drknoxy.eslint-disable-snippets)
- npm Intellisense (christian-kohler.npm-intellisense)
- vscode-styled-components (styled-components.vscode-styled-components)
