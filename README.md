# kotlin-runner

this is a reference for a bare minium toolset for messing around with kotlin at the CLI. it takes a single kotlin file and executes it, similar to how other interpreters might. this is useful for CLI enthusiasts curious about kotlin would want to experiment with the basics.

## usage

```
$ echo 'fun main() { println("hello") }' > /tmp/hello.kt
$ tsk run -- /tmp/hello.kt
hello
```

## deps

- tsk: the task-runner used. install with `brew install notnmeyer/tsk/tsk`.
  - technically optional. you can run `tsk/run` directly if you prefer.
- nix: `flake.nix` contains the kotlin and jvm dependencies. you don't need to use nix for these and can use it as a reference for what to install with your package manager of choice if you prefer.
