# @patrtorg/cupiditate-molestias-itaque

[![npm](https://img.shields.io/npm/v/@patrtorg/cupiditate-molestias-itaque)](https://www.npmjs.com/package/@patrtorg/cupiditate-molestias-itaque)

`@patrtorg/cupiditate-molestias-itaque` is a node command line tool to generate directory structure tree.

## Installation

```bash
npm i @patrtorg/cupiditate-molestias-itaque -g
```

## Usage

```bash
$ @patrtorg/cupiditate-molestias-itaque -h
Usage: @patrtorg/cupiditate-molestias-itaque [options]

Generate a directory structure tree

Options:
  -V, --version          output the version number
  -i, --ignore <ig>      ignore specific directory name, separated by comma or '|'  
  -l, --layer <layer>    specify the layer of output
  -d, --directory <dir>  specify the directory to generate structure tree
  -f, --only-folder      output folder only
  --icon                 output emoji icon, prefixing filename or directory
  -o, --output <output>  export content into a file, appending mode by default      
  -h, --help             display help for command
```

## Examples

Ignore `.git` and `node_modules` directory.

```bash
$ @patrtorg/cupiditate-molestias-itaque -i '.git|node_modules' # or @patrtorg/cupiditate-molestias-itaque -i '.git,node_modules'
@patrtorg/cupiditate-molestias-itaque
├──📄.editorconfig
├──📄.eslintrc.js
├──📄.gitignore
├──📄.prettierrc.js
├──📄.release-it.json
├──📄CHANGELOG.md
├──📄LICENSE
├──📄package-lock.json
├──📄package.json
├──📄README.md
└──📁src
    ├──📄config.js
    ├──📄generate.js
    ├──📄index.js
    ├──📄toTree.js
    └──📄utils.js
```

Show emoji icon, prefixing filename or directory.

```bash
$ @patrtorg/cupiditate-molestias-itaque -i '.git,node_modules' --icon
@patrtorg/cupiditate-molestias-itaque
├──📄.editorconfig
├──📄.eslintrc.js
├──📄.gitignore
├──📄.prettierrc.js
├──📄.release-it.json
├──📄CHANGELOG.md
├──📄LICENSE
├──📄package-lock.json
├──📄package.json
├──📄README.md
└──📁src
    ├──📄config.js
    ├──📄generate.js
    ├──📄index.js
    ├──📄toTree.js
    └──📄utils.js
```

Export output into `result.md`, and append mode by default.

```bash
$ @patrtorg/cupiditate-molestias-itaque -i '.git,node_modules' -o result.md
@patrtorg/cupiditate-molestias-itaque
├──📄.editorconfig
├──📄.eslintrc.js
├──📄.gitignore
├──📄.prettierrc.js
├──📄.release-it.json
├──📄CHANGELOG.md
├──📄LICENSE
├──📄package-lock.json
├──📄package.json
├──📄README.md
└──📁src
    ├──📄config.js
    ├──📄generate.js
    ├──📄index.js
    ├──📄toTree.js
    └──📄utils.js
```
## License

[MIT](./LICENSE)
