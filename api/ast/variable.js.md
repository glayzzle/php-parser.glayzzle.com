<a name="Variable"></a>

## Variable ⇐ <code>Expression</code>
**Kind**: global class  
**Extends**: <code>Expression</code>  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| name | <code>String</code> \| <code>Node</code> | The variable name (can be a complex expression when the name is resolved dynamically) |
| byref | <code>boolean</code> | Indicate if the variable reference is used, ex `&$foo` |
| curly | <code>boolean</code> | Indicate if the name is defined between curlies, ex `${foo}` |

