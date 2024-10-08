# Rizon language

![Picture](icon.png){ width="200" height="200" style="display: block; margin: 0 auto" }

## Interpreted language for fast iteration and type safety

>[!IMPORTANT]
>Rizon is still in development, use it for personal purpose only.
>
>It is entirely made by my self in my free time. If you want to give it a try and report any bug fell free to do so.

Rizon is a language that aims to be handful for quick prototyping thanks to type inference and cohercion and light syntax while being type safe, preventing lots of runtime crash.

The language is not OOP but it lets you define fields and methods on structures. To define common behavior, you have to define trait on structures.

Right know the interpreter walks an AST generated by a recursive descent parser. This is not optimal as it is slow, in the future it will be implemented as a bytecode compiler running on its own Rust VM.

## Main features

In its current state, you can acheive all the basic stuff you would expect from a language:

- Arithmetic operations
- User defined functions
- String manipulation

It also already has more advanced features:

- Structures
- Type safety at compile time
- First class function
- Closures
- Type inference
- Flow sensitive typing

Its current standard library is pretty poor, more to come in the future. Regarding the documentation, it's also under development.

## Future features

To acheive its goal, the language is going to need to support more complex features such as:

- Type unions
- Nullable types
- Errors as value
- Generic types
- Enums and pattern matching
- Traits
- Private methods and fields
- Modules
- Standard library

## CLI usage

You can use ```rizon.exe``` command alone to enter REPL mode.

You can pass additional arguments:
| Shorthand | Full             | Description                                                               | Default |
|-----------|------------------|---------------------------------------------------------------------------|---------|
| -f        | --file           | path to the file to run                                                   | ""      |
| -i        | --inter          | enters REPL mode after executing file                                     | false   |
|           | --print-tokens   | prints the output of the lexer                                            | false   |
| -s        | --static-analyse | only runs the static analysis (lexer, parser, static analyzer)            | false   |
| -h        | --help           | shows help message and exits                                              | false   |
| -v        | --version        | prints version information and exits                                      | false   |

## Tools

You can use the official VSCode plugin to work with the language to have basic language support. You can find the **vsix** file in the official repo: [rizon-vscode-tools](https://github.com/MartinVacheron/rizon-vscode-tools).

## Road map

Big features programmed for the following versions

### Rizon v0.2

- [ ] ```break``` statement in for and while loops
- [ ] ```else if``` branch
- [ ] Scientific notation for ```int``` and ```float``` (1e-4)
- [ ] Ternary operator: ```var a = foo == bar ? 1 : 0```
- [ ] Compound assign: ```a += 1```
- [ ] Comma declaration for variables: ```var a, b, c: int```
- [ ] Range with expressions
- [ ] Enums
- [ ] Upgrade global performance

### Rizon v0.3

- [ ] Type union
- [ ] Generic type
- [ ] Array built-in type

### Rizon v0.4

- [ ] Error type
- [ ] Error type union
- [ ] ```try```, ```or```, ```then``` keywords for erros

### Rizon v0.5

- [ ] ```match``` statements
- [ ] Flow sensitive typing

### Rizon v0.6

- [ ] Modules
- [ ] Rich standard library
- [ ] Standard library separated in modules

### Rizon v1.0

- [ ] Cleanup
- [ ] Bug fix
- [ ] Performance

## Credits

The logo was made with [GodSVG](https://github.com/MewPurPur/GodSVG).
