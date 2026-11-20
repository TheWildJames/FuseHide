# FuseHide 1.214

- **Version:** `1.214`
- **VersionCode:** `214`
- **Commit:** [`3192cba`](https://github.com/TheWildJames/FuseHide/commit/3192cba47ceacdd9665b5545b0ea5e2766734687)
- **Build time:** `9m 56s`
- **SHA256:** `eb49f5ffe7464a0127e10062c3514129ebb5d41481d8e22cb1648a53b212acba`

## Message

```text
fix(ui): stop prefixing relative paths with '|' in per-app subdirectory editor

appSpecificTargetsText() rendered every hiddenRelativePaths entry as
'|<path>', so re-opening an app's config showed e.g.
'|Android/data/com.rifsxd.ksunext'. The marker is redundant: the parser
already classifies targets by '/' and strips a leading '|', so it only
leaked noise into the editor text (and into the saved config if copied
to the global targets field).

```
