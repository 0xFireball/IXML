
# IXML

An extensible markup language. A partial reimplementation of Jade/Pug. Far more concise than XML

## About

**IXML** is based on my previous work on [KJade](https://github.com/0xFireball/KJade), which could compile a subset of Jade/Pug to XML.
IXML is a more generalized and improved version of KJade.

## How it works

**IXML** is composed of a number of components that sequentially run on intermediate representations of the input.
Algorithmically, it makes heavy use of recursion to efficiently build an abstract syntax tree. This representation can then
be used to generate code in XML or other forms, again using recursion.

1. A Lexer component walks through the source and uses regular expressions to turn the input into a list of tokens.
1. A Parser component takes tokens and uses the tokens to put together an abstract syntax tree, consisting of a hierarchy of nodes.
1. A Compiler component uses the AST to recursively generate code in another markup language 


## License

Copyright &copy; 2016 0xFireball, IridiumIon Software. All Rights Reserved.  
Licensed under the Apache License 2.0
