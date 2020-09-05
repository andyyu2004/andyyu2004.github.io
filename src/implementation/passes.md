# Passes

The L compiler is currently a pass based compiler. The passes are
currently approximately as follows:

- Lexical Analysis: `source code -> token stream`
- Parsing: `token stream -> abstract syntax tree`
- AST Lowering: `AST -> IR`
- Typechecking: `IR -> Typed IR (TIR)`
- TIR Lowering: `TIR -> Midlevel IR (MIR)`
- MIR Lowering: `MIR -> LLVM IR`
- Code Generation: `LLVM IR -> Output`


