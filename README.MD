# NodeJS - Next Level Week 6ª edição

  - Extensões: ESLint | Prettier - Code formatter

## Instalação das ferramentas

  - [Tutorial](https://www.notion.so/Instala-o-das-ferramentas-e5daec61d6a74da19486ad862027529e)
  
  - npm install --global yarn
  
  - Fonte: JetBrains Mono
  
    - https://www.jetbrains.com/lp/mono/
	- Após baixar, extraia o arquivo e acesse a pasta ttf
	- LINUX: Extraia as fontes para ~/.local/share/fonts ou /usr/share/fonts para instalar as fontes no sistema e execute fc-cache -f -v no terminal
  
  - Configurar Font Ligatures no VSCODE
  
  - Extensões: Omni Theme (baseado no Dracula) | Material Icon Theme
  
  - Ctrl + Shift + P \ Open Settings (JSON)
  
```json
{
  // Configurações da fonte JetBrains Mono
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,

  // Demais configurações
  "workbench.colorTheme": "Omni",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.startupEditor": "newUntitledFile",

  "explorer.compactFolders": false,
  "editor.renderLineHighlight": "gutter",
  "workbench.editor.labelFormat": "short",
  "extensions.ignoreRecommendations": true,

  "javascript.updateImportsOnFileMove.enabled": "always",
  "typescript.updateImportsOnFileMove.enabled": "never",

  "breadcrumbs.enabled": true,
  "editor.parameterHints.enabled": false,
  "editor.formatOnSave": true,
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,

  "emmet.syntaxProfiles": { "javascript": "jsx" },
  "emmet.includeLanguages": { "javascript": "javascriptreact" },

  "javascript.suggest.autoImports": true,
  "typescript.suggest.autoImports": true,
}  
```

É preciso tomar alguns cuidados ao realizar essas alterações. Verifique se a configuração adicionada já não existe no arquivo. Se sim, apenas atualize o valor. 

Verifique também se a todas as linhas de configuração **exceto a última terminam com vírgula**, para não gerar erro.


## Configurações do ambiente

  - [Tutorial](https://www.notion.so/Configura-es-do-ambiente-45e12d2ced17465cabbd81dcbd53576d)

  - Extensões: Code Spell Checker | Portuguese - Code Spell Checker | Color Highlight
	
  - Ctrl + Shift + P \ Preferences: Open Settings (JSON) 

```json
 {
	 "terminal.integrated.fontSize": 14,

	"editor.tabSize": 2,
	"editor.fontSize": 16,
	"editor.lineHeight": 26,
	"editor.semanticHighlighting.enabled": false,

	"editor.rulers": [80, 120],

	"editor.codeActionsOnSave": {
	  "source.fixAll.eslint": true
	},

	"files.associations": {
	  ".sequelizerc": "javascript",
	  ".stylelintrc": "json",
	  ".prettierrc": "json",
	  "*.tsx": "typescriptreact"
	},

	"typescript.tsserver.log": "verbose",
	"material-icon-theme.activeIconPack": "nest",

	"material-icon-theme.folders.associations": {
	  "infra": "app",
	  "entities": "class",
	  "domain": "class",
	  "schemas": "class",
	  "typeorm": "database",
	  "repositories": "mappings",
	  "http": "container",
	  "migrations": "tools",
	  "modules": "components",
	  "implementations": "core",
	  "dtos": "typescript",
	  "fakes": "mock",
	  "websockets": "pipe",
	  "protos": "pipe",
	  "grpc": "pipe",
	  "providers": "include",
	  "subscribers": "messages",
	  "useCases": "controller",
	  "kafka": "scripts",
	  "mappers": "meta",
	  "_shared": "shared",
	  "eslint-config": "tools",
	  "kube": "kubernetes"
	},

	"material-icon-theme.files.associations": {
	  "ormconfig.json": "database",
	  "tsconfig.json": "tune",
	  "*.proto": "3d",
	  "*.webpack.js": "webpack"
	},
	"window.menuBarVisibility": "toggle",
	"cSpell.enableFiletypes": [
	  "!asciidoc",
	  "!c",
	  "!cpp",
	  "!csharp",
	  "!go",
	  "!handlebars",
	  "!haskell",
	  "!jade",
	  "!java",
	  "!latex",
	  "!php",
	  "!pug",
	  "!python",
	  "!restructuredtext",
	  "!rust",
	  "!scala",
	  "!scss"
	],
	"cSpell.language": "en,pt",
	"editor.suggestSelection": "first",
	"cSpell.userWords": [
	  "chakra",
	  "middlewares",
	  "prefetch",
	  "rocketseat"
	],
	"workbench.productIconTheme": "fluent-icons",
	"terminal.integrated.showExitAlert": false,

	"splitHTMLAttributes.closingBracketOnNewLine": true,
	"window.zoomLevel": 1
}
 
```

## Atualizações

  - [Tutorial](https://www.notion.so/Atualiza-o-vers-es-diferentes-8b8cc815c02f4a9a8f0605422dd735ee)