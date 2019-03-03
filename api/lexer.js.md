<a name="lexer"></a>

## lexer
**Kind**: global class  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| EOF | <code>Integer</code> |  |
| all_tokens | <code>Boolean</code> | defines if all tokens must be retrieved (used by token_get_all only) |
| comment_tokens | <code>Boolean</code> | extracts comments tokens |
| mode_eval | <code>Boolean</code> | enables the evald mode (ignore opening tags) |
| asp_tags | <code>Boolean</code> | disables by default asp tags mode |
| short_tags | <code>Boolean</code> | enables by default short tags mode |
| keywords | <code>Object</code> | List of php keyword |
| castKeywords | <code>Object</code> | List of php keywords for type casting |


* [lexer](#lexer)
    * [.setInput()](#lexer+setInput)
    * [.input()](#lexer+input)
    * [.unput()](#lexer+unput)
    * [.getState()](#lexer+getState)
    * [.setState()](#lexer+setState)

<a name="lexer+setInput"></a>

### lexer.setInput()
Initialize the lexer with the specified input

**Kind**: instance method of [<code>lexer</code>](#lexer)  
<a name="lexer+input"></a>

### lexer.input()
consumes and returns one char from the input

**Kind**: instance method of [<code>lexer</code>](#lexer)  
<a name="lexer+unput"></a>

### lexer.unput()
revert eating specified size

**Kind**: instance method of [<code>lexer</code>](#lexer)  
<a name="lexer+getState"></a>

### lexer.getState()
Gets the current state

**Kind**: instance method of [<code>lexer</code>](#lexer)  
<a name="lexer+setState"></a>

### lexer.setState()
Sets the current lexer state

**Kind**: instance method of [<code>lexer</code>](#lexer)  
