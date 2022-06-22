## Opening an issue


### Scala 3 version

The version of Scala 3 in which the bug is found.

This field may must contain one or more (comma separated) versions of the compiler
- `3.x.y`
- `3.x.y-RCn`
- `3.x.y-RCn-bin-date-hash-NIGHTLY`
- `hash`

If you're not sure what version you're using, run `print scalaVersion` from sbt (if you're running scalac manually, use `scalac -version` instead).

### Last good version

Last good version if this bug is a regression.

By default the value is `None` indicating this is not a regression. Otherwise should contain a version formatted as in _Scala 3 version_ section.

### How to reproduce the bug

TODO

### Expected behavior

Describe the expected behavior. For example:

- It should compile and produce code equivalent to ...
- The generated code should run and produce ...
- It should emit an error (or warning) at ... stating that ...
- It should compile faster ...

### Ease of reproduction

Select all options that apply.

- Reproducible:
  We have access to code and command that allow the issue to be reproduced.
  The code may be in a brach of the project that failed or in a smaller example.
  The code may have external dependencies.

- Reproducible without external dependencies: Same as _reproducible_ but without any external dependencies. This implies that there is a simple project or multi-project that contains all the code needed to reproduce the issue.

- Reproducible with self-contained example: The code is one (or a few) source files and can be reproduces with `scalac`/`sclala`.

- Reproducible with minimal example: The example is self-contained and does not contain any irrelevant code or language features. This can be achieved by:
  - Trying to remove implementation
  - Trying to remove parameters
  - Trying to remove definitions
  - Trying to use normal classes instead of case classes
  - Trying to use explicit types instead of inferred types
  - Trying to use implicits explicitly
  - Trying to remove `inline` keyword
  - Trying to remove macros


### Fixing the issue

One should not try to modify the code of the compile or library before understanding the source of the issue and how it can be fixed. The usual steps to follow are:

- Identify source of the issue
- Identify a possible solution
- Add example form from the issue as tests and make sure the issue is identified by the testing framework
- Add more tests that could exhibit similar issues (even if those currently work)
- Implement the solution
