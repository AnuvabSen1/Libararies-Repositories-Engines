# Libraries-Repositories-Engine

Every hour, the automated Library Manager indexer system runs this tool, which:

1. checks every repository in the [Library Manager list]() for new [tags]()
1. checks whether those tags meet [the requirements for addition to the index](), publishing [logs]()
1. adds entries to the index for compliant tags
1. pushes the updated index to Arduino's download server

## BUILD

```
task go:build
```

## TDD

In order to run the tests, type

```
task go:test
```

## RUN

Create a `config.json` file (or edit example one). Same thing for `repos.txt` file.

Run with `go run sync_libraries.go` or `task go:build` and then `./libraries-repository-engine`

## Security

If you think you found a vulnerability or other security-related bug in this project, please read our
[security policy](https://github.com/AnuvabSen/Libararies-Repositories-Engines/edit/master/README.md) please inform me.
Thank you!
