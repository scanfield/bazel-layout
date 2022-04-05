### Confusing gazelle layout

In this repo, there is a top level `go` directory, and all go source code is under that. Not present in this example but imagine top level `rust` or `proto` directories as well.

I am having trouble getting the generated "importpath" to work properly. Either I set -repo_root to the go/src/ directory and end up with importpaths like `github.com/mypackage/github.com/mypackage/baz` or I leave it unset and get importpaths like `github.com/mypackage/go/src/github.com/mypackage/baz`.

What I want is importpath like `github.com/mypackage/baz`.