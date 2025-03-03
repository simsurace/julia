Julia v1.10 Release Notes
========================

New language features
---------------------

Language changes
----------------


Compiler/Runtime improvements
-----------------------------


Command-line option changes
---------------------------


Multi-threading changes
-----------------------


Build system changes
--------------------


New library functions
---------------------
* `tanpi` is now defined. It computes tan(πx) more accurately than `tan(pi*x)` ([#48575]).

New library features
--------------------
* The `initialized=true` keyword assignment for `sortperm!` and `partialsortperm!`
  is now a no-op ([#47979]). It previously exposed unsafe behavior ([#47977]).
* `binomial(x, k)` now supports non-integer `x` ([#48124]).
* A `CartesianIndex` is now treated as a "scalar" for broadcasting ([#47044]).

Standard library changes
------------------------


#### Package Manager

- "Package Extensions": support for loading a piece of code based on other
  packages being loaded in the Julia session.
  This has similar applications as the Requires.jl package but also
  supports precompilation and setting compatibility.
#### LinearAlgebra


#### Printf
* Format specifiers now support dynamic width and precision, e.g. `%*s` and `%*.*g` ([#40105]).

#### Profile


#### Random


#### REPL


#### SuiteSparse


#### SparseArrays


#### Test


* The `@test_broken` macro (or `@test` with `broken=true`) now complains if the test expression returns a
  non-boolean value in the same way as a non-broken test. ([#47804])

#### Dates


#### Distributed


#### Unicode


#### DelimitedFiles


#### InteractiveUtils

 * `code_native` and `@code_native` now default to intel syntax instead of AT&T.

Deprecated or removed
---------------------


External dependencies
---------------------


Tooling Improvements
--------------------


<!--- generated by NEWS-update.jl: -->
