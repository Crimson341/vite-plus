# create_npm_inherited_npx_env

npx-inherited npm_config_package must not leak into the nested `npx create-vite` (#2970).

## `vp create vite:application --no-interactive --directory my-app --no-agent --no-editor --no-hooks`


## `vpt stat-file my-app/package.json --assert file`

app was scaffolded

```
my-app/package.json: file
```
