# Crucible Snap

This snap provides an easy way to install and run the tests found in
[Mesa's Crucible Vulkan Test Suite](https://gitlab.freedesktop.org/mesa/crucible).

## Build

```
snapcraft pack
```

## Install

```
snap install --dangerous crucible_git_<your_arch>.snap
```

## Run

### List available tests
```
crucible.list-tests
```

### Run tests

Run a specific test:
```
crucible.test func.spirv.foo
```

Run tests matching a pattern:
```
crucible.test 'func.*'
```

Results are written to `~/.crucible/results.xml` in JUnit XML format.
