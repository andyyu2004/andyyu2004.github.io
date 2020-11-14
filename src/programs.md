# L Programs

> **Syntax**
>
> &lt;program&gt; ::= <*[module]*>

An L program consists of a collection of items where one of them is the
main function.

The compiler requires a top level configuration file `L.toml`. The path
of this configuration file or the path of its parent directory should be
passed to the compiler to compile the program. We call each program
with its associated `L.toml` file a "package".


The following is an example of a minimal `L.toml`.

```
# L.toml

[package]
name = "foo"
version = "0.1.0"
```


[module]: modules.md
