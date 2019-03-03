## Classes

<dl>
<dt><a href="#ClassReference">ClassReference</a> ⇐ <code>Reference</code></dt>
<dd></dd>
</dl>

## Constants

<dl>
<dt><a href="#UNQUALIFIED_NAME">UNQUALIFIED_NAME</a> : <code>String</code></dt>
<dd><p>This is an identifier without a namespace separator, such as Foo</p>
</dd>
<dt><a href="#QUALIFIED_NAME">QUALIFIED_NAME</a> : <code>String</code></dt>
<dd><p>This is an identifier with a namespace separator, such as Foo\Bar</p>
</dd>
<dt><a href="#FULL_QUALIFIED_NAME">FULL_QUALIFIED_NAME</a> : <code>String</code></dt>
<dd><p>This is an identifier with a namespace separator that begins with
a namespace separator, such as \Foo\Bar. The namespace \Foo is also
a fully qualified name.</p>
</dd>
<dt><a href="#RELATIVE_NAME">RELATIVE_NAME</a> : <code>String</code></dt>
<dd><p>This is an identifier starting with namespace, such as namespace\Foo\Bar.</p>
</dd>
</dl>

<a name="ClassReference"></a>

## ClassReference ⇐ <code>Reference</code>
**Kind**: global class  
**Extends**: <code>Reference</code>  
**Properties**

| Name | Type |
| --- | --- |
| name | <code>string</code> | 
| resolution | <code>string</code> | 

<a name="UNQUALIFIED_NAME"></a>

## UNQUALIFIED\_NAME : <code>String</code>
This is an identifier without a namespace separator, such as Foo

**Kind**: global constant  
<a name="QUALIFIED_NAME"></a>

## QUALIFIED\_NAME : <code>String</code>
This is an identifier with a namespace separator, such as Foo\Bar

**Kind**: global constant  
<a name="FULL_QUALIFIED_NAME"></a>

## FULL\_QUALIFIED\_NAME : <code>String</code>
This is an identifier with a namespace separator that begins with
a namespace separator, such as \Foo\Bar. The namespace \Foo is also
a fully qualified name.

**Kind**: global constant  
<a name="RELATIVE_NAME"></a>

## RELATIVE\_NAME : <code>String</code>
This is an identifier starting with namespace, such as namespace\Foo\Bar.

**Kind**: global constant  
