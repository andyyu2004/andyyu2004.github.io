# Modules

> **Syntax**
>
> <*module*> ::= <*[item]*><sup>*</sup>
>
> <*module-decl*> ::= `mod` <*ident*>;
>

The top level program is an implicit root module.

Within it, we can declare submodules with the module declaration item:
`mod foo`.

Consider the following example:

```
// src/main.l

mod foo;

fn main() {
    ...
}

```

The `foo` module will be searched for in either `src/foo.l` or
`src/foo/foo.l`. In the former case, we call `foo` a "file module", and
in the latter case, we call it a "directory module". Only directory
modules are allowed to have submodules.


[item]: items.md

