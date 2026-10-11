# vp_no_header_local

## `vp hooks -h`

banner by default

```
VITE+ - The Unified Toolchain for the Web

Usage: vp hooks <COMMAND> [OPTIONS]

Manage the Vite+ Git hook dispatcher for this repository.

Options:
  -h, --help  Show this help message

Commands:
  enable   Install or refresh the hook dispatcher (sets core.hooksPath)
  disable  Disable hooks: unset core.hooksPath, remove <dir>/_, persist preference
  status   Show preference, core.hooksPath, and dispatcher state

Environment:
  VP_GIT_HOOKS=0  Skip dispatcher install in enable (and skip hooks at commit time)

Examples:
  vp hooks enable
  vp hooks enable --hooks-dir .custom-hooks
  vp hooks disable
  vp hooks status

Documentation: https://viteplus.dev/guide/commit-hooks
```

## `VP_NO_HEADER=1 vp hooks -h`

no banner

```
Usage: vp hooks <COMMAND> [OPTIONS]

Manage the Vite+ Git hook dispatcher for this repository.

Options:
  -h, --help  Show this help message

Commands:
  enable   Install or refresh the hook dispatcher (sets core.hooksPath)
  disable  Disable hooks: unset core.hooksPath, remove <dir>/_, persist preference
  status   Show preference, core.hooksPath, and dispatcher state

Environment:
  VP_GIT_HOOKS=0  Skip dispatcher install in enable (and skip hooks at commit time)

Examples:
  vp hooks enable
  vp hooks enable --hooks-dir .custom-hooks
  vp hooks disable
  vp hooks status

Documentation: https://viteplus.dev/guide/commit-hooks
```

## `VP_NO_HEADER=1 vp help dev`

no banner

```
Usage: vp dev [ROOT] [OPTIONS]

Run the development server.
Options are forwarded to Vite.

Arguments:
  [ROOT]  Project root directory (default: current directory)

Options:
  --host [host]           [string] specify hostname
  --port <port>           [number] specify port
  --open [path]           [boolean | string] open browser on startup
  --cors                  [boolean] enable CORS
  --strictPort            [boolean] exit if specified port is already in use
  --force                 [boolean] force the optimizer to ignore the cache and re-bundle
  --experimentalBundle    [boolean] use experimental full bundle mode (this is highly experimental)
  --base <path>           [string] public base path (default: /)
  -l, --logLevel <level>  [string] info | warn | error | silent
  --clearScreen           [boolean] allow/disable clear screen when logging
  -d, --debug [feat]      [string | boolean] show debug logs
  -f, --filter <filter>   [string] filter debug logs
  -m, --mode <mode>       [string] set env mode
  -h, --help              Display this message

Examples:
  vp dev
  vp dev --open
  vp dev --host localhost --port 5173

Documentation: https://viteplus.dev/guide/dev
```
