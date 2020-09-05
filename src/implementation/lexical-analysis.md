# Lexical Analysis

The lexer breaks the input source (`&str`) into a sequence of tokens.
The lexer uses a simple library that is also utilised in the rustc
compiler which returns an iterator of `TokenKind`s. This is then
transformed into my representation of Tokens and returned as a Vector.

Importantly, the lexer maintains the positions of each token in the
source code by keeping track of the `Span`. A `Span` is nothing more
than the start (inclusive) and end (exclusive) index of the token in the
input string.

The relevant source code can be found in the
[lexer](https://gitlab.com/andyyu2004/vm/-/tree/master/src/vm/src/lexer)
module.
