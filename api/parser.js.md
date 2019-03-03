## Constants

<dl>
<dt><a href="#ignoreStack">ignoreStack</a></dt>
<dd><p>outputs some debug information on current token</p>
</dd>
</dl>

## parser


<a name="parser"></a>

**Kind**: global class  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| lexer | <code>Lexer</code> | current lexer instance |
| ast | <code>AST</code> | the AST factory instance |
| token | <code>Integer</code> \| <code>String</code> | current token |
| extractDoc | <code>Boolean</code> | should extract documentation as AST node |
| extractTokens | <code>Boolean</code> | should extract each token |
| suppressErrors | <code>Boolean</code> | should ignore parsing errors and continue |
| debug | <code>Boolean</code> | should output debug informations |


* [parser](#parser)
    * [.getTokenName()](#parser+getTokenName)
    * [.parse()](#parser+parse)
    * [.raiseError()](#parser+raiseError)
    * [.error()](#parser+error)
    * [.node()](#parser+node)
    * [.expectEndOfStatement()](#parser+expectEndOfStatement) ⇒ <code>boolean</code>
    * [.expect(token)](#parser+expect) ⇒ <code>boolean</code>
    * [.text()](#parser+text) ⇒ <code>String</code>
    * [.next()](#parser+next)
    * [.lex()](#parser+lex)
    * [.is()](#parser+is)

<a name="parser+getTokenName"></a>

### parser.getTokenName()
helper : gets a token name

**Kind**: instance method of [<code>parser</code>](#parser)  
<a name="parser+parse"></a>

### parser.parse()
main entry point : converts a source code to AST

**Kind**: instance method of [<code>parser</code>](#parser)  
<a name="parser+raiseError"></a>

### parser.raiseError()
Raise an error

**Kind**: instance method of [<code>parser</code>](#parser)  
<a name="parser+error"></a>

### parser.error()
handling errors

**Kind**: instance method of [<code>parser</code>](#parser)  
<a name="parser+node"></a>

### parser.node()
Creates a new AST node

**Kind**: instance method of [<code>parser</code>](#parser)  
<a name="parser+expectEndOfStatement"></a>

### parser.expectEndOfStatement() ⇒ <code>boolean</code>
expects an end of statement or end of file

**Kind**: instance method of [<code>parser</code>](#parser)  
<a name="parser+expect"></a>

### parser.expect(token) ⇒ <code>boolean</code>
Force the parser to check the current token.

If the current token does not match to expected token,
the an error will be raised.

If the suppressError mode is activated, then the error will
be added to the program error stack and this function will return `false`.

**Kind**: instance method of [<code>parser</code>](#parser)  
**Throws**:

- Error


| Param | Type |
| --- | --- |
| token | <code>String</code> \| <code>Number</code> | 

<a name="parser+text"></a>

### parser.text() ⇒ <code>String</code>
Returns the current token contents

**Kind**: instance method of [<code>parser</code>](#parser)  
<a name="parser+next"></a>

### parser.next()
consume the next token

**Kind**: instance method of [<code>parser</code>](#parser)  
<a name="parser+lex"></a>

### parser.lex()
Eating a token

**Kind**: instance method of [<code>parser</code>](#parser)  
<a name="parser+is"></a>

### parser.is()
Check if token is of specified type
## Constants
stance method of [<code>parser</code>](#parser)  
<dl>oreStack"></a>
<dt><a href="#ignoreStack">ignoreStack</a></dt>
<dd><p>outputs some debug information on current token</p>ck
</dd> debug information on current token
</dl>
**Kind**: global constant  

## API

* [array.js](docs/api/array.js.md)
* [class.js](docs/api/class.js.md)
* [comment.js](docs/api/comment.js.md)
* [expr.js](docs/api/expr.js.md)
* [function.js](docs/api/function.js.md)
* [if.js](docs/api/if.js.md)
* [loops.js](docs/api/loops.js.md)
* [main.js](docs/api/main.js.md)
* [namespace.js](docs/api/namespace.js.md)
* [scalar.js](docs/api/scalar.js.md)
* [statement.js](docs/api/statement.js.md)
* [switch.js](docs/api/switch.js.md)
* [try.js](docs/api/try.js.md)
* [utils.js](docs/api/utils.js.md)
* [variable.js](docs/api/variable.js.md)