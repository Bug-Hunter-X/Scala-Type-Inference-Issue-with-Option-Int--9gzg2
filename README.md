# Scala Type Inference Issue with Option[Int]
This repository demonstrates a type inference issue in Scala when using `Option[Int]` as a type parameter for a generic class.  The code compiles and runs successfully with `Int`, `String`, and `List`, but fails with `Option[Int]`, resulting in a `MatchError`.

## Problem
The `MyClass` class is designed to hold a value of type `T`. When `T` is `Option[Int]`, the `printValue` method encounters an unexpected `MatchError`. This indicates that type inference isn't properly handling the `Option` type in this context.

## Solution
The solution involves explicitly handling the `Option` type within the `printValue` method using pattern matching.

## How to Reproduce
1. Clone this repository.
2. Compile and run `Main.scala`.
3. Observe the `MatchError` when the `myOption` instance is processed.
