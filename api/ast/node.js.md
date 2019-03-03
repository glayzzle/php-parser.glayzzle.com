<a name="Node"></a>

## Node
**Kind**: global class  
**Properties**

| Name | Type |
| --- | --- |
| loc | <code>Location</code> \| <code>null</code> | 
| leadingComments | <code>Array.&lt;Comment&gt;</code> | 
| trailingComments | <code>Array.&lt;Comment&gt;</code> | 
| kind | <code>String</code> | 


* [Node](#Node)
    * _instance_
        * [.setTrailingComments(docs)](#Node+setTrailingComments)
        * [.includeToken(parser)](#Node+includeToken)
    * _static_
        * [.extends(type, constructor)](#Node.extends) ⇒ <code>function</code>

<a name="Node+setTrailingComments"></a>

### node.setTrailingComments(docs)
Attach comments to current node

**Kind**: instance method of [<code>Node</code>](#Node)  

| Param | Type |
| --- | --- |
| docs | <code>\*</code> | 

<a name="Node+includeToken"></a>

### node.includeToken(parser)
Includes current token position of the parser

**Kind**: instance method of [<code>Node</code>](#Node)  

| Param | Type |
| --- | --- |
| parser | <code>\*</code> | 

<a name="Node.extends"></a>

### Node.extends(type, constructor) ⇒ <code>function</code>
Helper for extending the Node class

**Kind**: static method of [<code>Node</code>](#Node)  

| Param | Type |
| --- | --- |
| type | <code>String</code> | 
| constructor | <code>function</code> | 

