# cs51-project
Implementing a subset of OCaml and a simple version of the REPL, called miniml. 

### Requirements
Just the code and a terminal where you can run it. Use the command `ocamlbuild  -use-ocamlfind  miniml.byte` to build the project, then run it with `./miniml.byte`. 

### Description
This was my final project for Harvard's CS51. It involved implementing REPL functionality to work with various data types and unary and binary operators. The implementation makes use of various semantics regimes, including substitution, dynamic, and lexical.

The main components of this project were deciding how functions, let statements, conditionals, function applications, recursive functions, etc. were to be handled under each semantics scheme. This involved careful thought about how to handle expressions recursively such that we can account for perhaps very long functions with nested expressions. In order to get a working REPL, I adapted the parser to work with various data types. For example, as an extension for the project, I implemented functionality for handing floating-point values, which required that I adapt the parser to also handle these values as they are read in from the REPL. 
