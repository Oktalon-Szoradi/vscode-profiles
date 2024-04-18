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
  "accessibility.voice.keywordActivation": "chatInContext",
  "dotenv.enableAutocloaking": true,
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
    "textMateRules": [
      {
        "scope": "keyword.other.dotenv",
        "settings": {
          "foreground": "#FF000000"
        }
      }
    ]
  },
  "editor.wordWrap": "off",
  "eslint.format.enable": true,
  "files.associations": {
    ".env*": "dotenv"
  },
  "files.autoSave": "afterDelay",
  "git.autofetch": true,
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
  "terminal.integrated.defaultProfile.windows": "Git Bash",
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

- Vue - Official (Vue.volar)
- Auto Import (steoates.autoimport)
- Better Comments (aaron-bond.better-comments)
- Dotenv Official +Vault (dotenv.dotenv-vscode)
- Error Lens (usernamehw.errorlens)
- ESLint (dbaeumer.vscode-eslint)
- eslint-disable-snippets (drKnoxy.eslint-disable-snippets)
- htmltagwrap (bradgashler.htmltagwrap)
- Import Cost (wix.vscode-import-cost)
- indent-rainbow (oderwat.indent-rainbow)
- JavaScript Auto Backticks (chamboug.js-auto-backticks)
- JavaScript Booster (sburg.vscode-javascript-booster)
- Live Preview (ms-vscode.live-server)
- Material Icon Theme (PKief.material-icon-theme)
- Material Product Icons (PKief.material-product-icons)
- npm Intellisense (christian-kohler.npm-intellisense)
- Package Json Upgrade (codeandstuff.package-json-upgrade)
- REST Client (humao.rest-client)
- Sass (.sass only) (syler.sass-indented)
- SCSS Formatter (sibiraj-s.vscode-scss-formatter)
- Sort JSON objects (richie5um2.vscode-sort-json)
- Sort package.json (unional.vscode-sort-package-json)
- Stylelint (stylelint.vscode-stylelint)
- Surround (Sword.vscode-surround)
- Svg Preview (SimonSiefke.svg-preview)
- Toggle Quotes (BriteSnow.vscode-toggle-quotes)
- Twoslash Query Comments (Orta.vscode-twoslash-queries)
- Vitest (vitest.explorer)
- vscode-styled-components (styled-components.vscode-styled-components)
- Vue 3 Support - All In One (Wscats.vue)
- Vue VSCode Snippets (sdras.vue-vscode-snippets)
- GitHub Pull Requests (GitHub.vscode-pull-request-github)
- jsdoc (lllllllqw.jsdoc)
- Live Server (Five Server) (yandeu.five-server)

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
  "[markdown]": {
    "editor.defaultFormatter": "yzhang.markdown-all-in-one"
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
  "indentRainbow.ignoreErrorLanguages": [
    "*",
    "markdown"
  ],
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
  "scssFormatter.singleQuote": true,
  "scssFormatter.trailingComma": "none",
  "security.allowedUNCHosts": [
    "wsl.localhost"
  ],
  "standard.autoFixOnSave": true,
  "standard.enableGlobally": true,
  "terminal.integrated.defaultProfile.windows": "Git Bash",
  "terminal.integrated.fontFamily": "'Fira Code', 'monospace', monospace",
  "togglequotes.chars": [
    "\"",
    "'",
    "`"
  ],
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

- .gitignore Generator (piotrpalarz.vscode-gitignore-generator)
- .NET Install Tool (ms-dotnettools.vscode-dotnet-runtime)
- AsciiDoc (asciidoctor.asciidoctor-vscode)
- Auto Import (steoates.autoimport)
- Autoprefixer (mrmlnc.vscode-autoprefixer)
- Better Comments (aaron-bond.better-comments)
- C# (ms-dotnettools.csharp)
- CSS Flexbox Cheatsheet (dzhavat.css-flexbox-cheatsheet)
- CSS Formatter (aeschli.vscode-css-formatter)
- CSS sorter (zascal.CSS-sorter)
- Dotenv Official +Vault (dotenv.dotenv-vscode)
- Error Lens (usernamehw.errorlens)
- eslint-disable-snippets (drKnoxy.eslint-disable-snippets)
- Format Files (jbockle.jbockle-format-files)
- GitHub Copilot (GitHub.copilot)
- GitHub Copilot Chat (GitHub.copilot-chat)
- *GitHub Markdown Preview (bierner.github-markdown-preview)*
- Headwind (heybourn.headwind)
- HTML CSS Support (ecmel.vscode-html-css)
- htmltagwrap (bradgashler.htmltagwrap)
- Import Cost (wix.vscode-import-cost)
- intent-rainbow (oderwat.indent-rainbow)
- Javascript Auto Backticks (chamboug.js-auto-backticks)
- JavaScript Booster (sburg.vscode-javascript-booster)
- JavaScript Docstrings (Massi.javascript-docstrings)
- JavaScript standardjs styled snippets (capaj.vscode-standardjs-snippets)
- LaTeX Workshop (James-Yu.latex-workshop)
- Live Preview (ms-vscode.live-server)
- Live Server (ritwickdey.LiveServer)
- Live Share (ms-vsliveshare.vsliveshare)
- Markdown All in One (yzhang.markdown-all-in-one)
- Markdown Checkboxes (bierner.markdown-checkbox)
- Markdown Emoji (bierner.markdown-emoji)
- Markdown Footnotes (bierner.markdown-footnotes)
- Markdown PDF (yzane.markdown-pdf)
- Markdown Preview Github Styling (bierner.markdown-preview-github-styles)
- Markdown Preview Mermaid Support (bierner.markdown-mermaid)
- Markdown yaml Preamble (bierner.markdown-yaml-preamble)
- Marp for VS Code (marp-team.marp-vscode)
- Material Icon Theme (PKief.material-icon-theme)
- Material Product Icons (PKief.material-product-icons)
- npm Intellisense (christian-kohler.npm-intellisense)
- Package Json Upgrade (codeandstuff.package-json-upgrade)
- Path Intellisense (christian-kohler.path-intellisense)
- Prettier - Code formatter (esbenp.prettier-vscode)
- Prettier-Standard - JavaScript formatter (numso.prettier-standard-vscode)
- Pylance (ms-python.vscode-pylance)
- Python (ms-python.python)
- Python Debugger (ms-python.debugpy)
- Rainbow CSV (mechatroner.rainbow-csv)
- Remote - SSH (ms-vscode-remote.remote-ssh)
- Remote - SSH: Editing Configuration Files (ms-vscode-remote.remote-ssh-edit)
- Remote Explorer (ms-vscode.remote-explorer)
- REST Client (humao.rest-client)
- Sass (.sass only) (syler.sass-indented)
- SCSS Formatter (sibiraj-s.vscode-scss-formatter)
- Sort JSON objects (richie5um2.vscode-sort-json)
- Sort package.json (unional.vscode-sort-package-json)
- SQLite Viewer (qwtel.sqlite-viewer)
- StandardJS - JavaScript Standard Style (standard.vscode-standard)
- Stylelint (stylelint.vscode-stylelint)
- Surround (Sword.vscode-surround)
- SVG (jock.svg)
- Svg Preview (SimonSiefke.svg-preview)
- Tailwind CSS IntelliSense (bradlc.vscode-tailwindcss)
- Toggle Quotes (BriteSnow.vscode-toggle-quotes)
- Twoslash Query Comments (Orta.vscode-twoslash-queries)
- Vitest (vitest.explorer)
- vscode-styled-components (styled-components.vscode-styled-components)
- Vue - Official (Vue.volar)
- Vue 3 Support - All In One (Wscats.vue)
- *Vue Extension Box (MisterJ.vue-volar-extention-pack)*
- Vue Snippets StandardJS (andersonmfjr.vue-snippets-standardjs)
- Vue VSCode Snippets (sdras.vue-vscode-snippets)

Disabled:
- Bootstrap Class Autocomplete (torresgol10.bootstrap-class-autocomplete)
- Bootstrap IntelliSense (hossaini.bootstrap-intellisense)
- colorize (kamikillerto.vscode-colorize)
- ESLint (dbaeumer.vscode-eslint)
- Inline fold (moalamri.inline-fold)
- LTeX – LanguageTool grammar/spell checking (valentjn.vscode-ltex)
- Markdown Preview Enhanced (shd101wyy.markdown-preview-enhanced)
- Prettier ESLint (rvest.vs-code-prettier-eslint)
