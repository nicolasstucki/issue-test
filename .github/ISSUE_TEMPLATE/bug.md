---
name: "\U0001F41B Bug report"
about: Report a bug about the Dotty Scala 3 Compiler
title: ''
labels: itype:bug, stat:needs triage
assignees: ''

---

## Compiler version

Fails in: TODO <!-- 3.x.y, 3.x.y-RCn, 3.x.y-hash-NIGHTLY, hash -->
<!-- If you're not sure what version you're using, run `print scalaVersion` from sbt
     (if you're running scalac manually, use `scalac -version` instead). -->
     

<!-- IF IT IS A REGRESSION
     
     To figure out when the regression started consider using the following script from the dotty repo: https://github.com/lampepfl/dotty/blob/main/project/scripts/dottyCompileBisect.scala
-->
<!-- Worked in: 3.x.y -->
<!-- First bad nightly: 3.x.y-hash-NIGHTLY -->
<!-- First bad commit: hash -->


## Status

- [ ] Reproducible
      <!-- The issue as instructions on how to be reproduced -->
- [ ] Reproducible without external dependencies 
      <!-- There file or project without external dependencies reproduces the bug -->
- [ ] Reproducible with minimal example
      <!-- The issue has been distilled to a minimal example. This example should remove any language features or code that is not relevant to reproduce the issue. -->
- [ ] Identified source source of the issue
      <!-- The source of the issue is identified to come from a bug while typing, a buggy code transformation, bug in the runtime, ... -->
- [ ] Identified solution
      <!-- A possible solution or solution plan has been identified -->
- [ ] Implemented solution
      <!-- The solution has been implemented and contains tests for the buggy code -->

## Issue reproduction

<!-- This code should be self contained, compilable (with possible failures) and as small as possible.
     Ideally, we should be able to just copy this code in a file and run `scalac` (and maybe `scala`) to reproduce the issue.
-->

### Input
<!-- FILE OR FILES -->
<!-- Include full source with imports -->
<!-- Keep filename for reproduction -->
```scala
// Test.scala
// TODO: add code
```

<!-- SEPARATE COMPILATION
     If a file must be compiled before the other, use the `_N` suffix for the file name.
     For exmaple, if we have `Macro_1.sclala` and `Test_2.scala`, it means that we will 
     first compile `Macro_1.sclala` and then compile `Test_2.scala` with a dependency 
     on `Test_2.scala`. `Macro.sclala` and `Test.scala` means that we compile both at 
     the same time (for macros avoid this one unless it is the only way to reproduce 
     the issue).
-->

<!-- BACKWARDS COMPAT: If a dependency must be compiled with an older version of the compiler, use the `_c3.x.y` suffix to indicate the older version (in combination with `_N`) -->


### Reproduction
<!-- EXPLAIN HOW TO REPRODUCE THE ISSUE -->

`scalac Test.scala`

<!-- IF IS A REPL ISSUE -->
<!-- 
```scala
// REPL
> // Code
```
-->

### Output

```
// TODO
```

<!-- IF THE OUTPUT CONTAINS A STACK TRACE IS TOO LONG -->
<!--
<details>
<summary>Detailed Output</summary>

```scala
// TODO add output here
```
</details>
-->

## Expected behavior

<!-- Describe the expected behaviour -->
