# vp_no_header

`VP_NO_HEADER` hides the banner in an interactive terminal (#2242).

## `vp fmt src/`

banner by default

```
VITE+ - The Unified Toolchain for the Web

Finished in <duration> on 1 files using <n> threads.
No config found, using defaults. Please add a config file or try `vp fmt --init` if needed.
```

## `VP_NO_HEADER=1 vp fmt src/`

no banner

```
Finished in <duration> on 1 files using <n> threads.
No config found, using defaults. Please add a config file or try `vp fmt --init` if needed.
```

## `VP_NO_HEADER=1 vp lint src/`

no banner

```
Found 0 warnings and 0 errors.
Finished in <duration> on 1 file with <n> rules using <n> threads.
```

## `VP_NO_HEADER=1 vp help`

no banner in help

```

Usage: vp [COMMAND]

Start:
  create      Create a new project from a template
  migrate     Migrate an existing project to Vite+
  config      Configure hooks and agent integration
  hooks       Manage the Git hook dispatcher
  staged      Run linters on staged files
  install, i  Install all dependencies, or add packages if package names are provided
  env         Manage Node.js and package managers

Develop:
  dev          Run the development server
  check        Run format, lint, and type checks
  lint         Lint code
  fmt, format  Format code
  test         Run tests

Execute:
  run    Run tasks (also available as standalone `vpr`)
  exec   Execute a command from local node_modules/.bin
  node   Run a Node.js script (shorthand for `env exec node`)
  dlx    Execute a package binary without installing it as a dependency
  cache  Manage the task cache

Build:
  build    Build for production
  pack     Build library
  preview  Preview production build

Manage Dependencies:
  add                        Add packages to dependencies
  remove, rm, un, uninstall  Remove packages from dependencies
  update, up                 Update packages to their latest versions
  dedupe                     Deduplicate dependencies by removing older versions
  outdated                   Check for outdated packages
  list, ls                   List installed packages
  why, explain               Show why a package is installed
  info, view, show           View package information from the registry
  link, ln                   Link packages for local development
  unlink                     Unlink packages
  rebuild                    Rebuild native modules
  pm                         Forward a command to the package manager

Maintain:
  toolchain  Show active Vite+ tools, versions, and relationships
  upgrade    Update vp itself to the latest version
  implode    Remove vp and all related data

Documentation: https://viteplus.dev/guide/

Options:
  -V, --version  Print version
  -C <DIR>       Run as if vp was started in <DIR> instead of the current working directory
  -h, --help     Print help
```
