## Classes

<dl>
<dt><a href="#Declare">Declare</a> ⇐ <code>Block</code></dt>
<dd></dd>
</dl>

## Constants

<dl>
<dt><a href="#MODE_SHORT">MODE_SHORT</a> : <code>String</code></dt>
<dd><p>The node is declared as a short tag syntax :</p>
<pre><code class="lang-php">&lt;?php
declare(ticks=1):
// some statements
enddeclare;
</code></pre>
</dd>
<dt><a href="#MODE_BLOCK">MODE_BLOCK</a> : <code>String</code></dt>
<dd><p>The node is declared bracket enclosed code :</p>
<pre><code class="lang-php">&lt;?php
declare(ticks=1) {
// some statements
}
</code></pre>
</dd>
<dt><a href="#MODE_NONE">MODE_NONE</a> : <code>String</code></dt>
<dd><p>The node is declared as a simple statement. In order to make things simpler
children of the node are automatically collected until the next
declare statement.</p>
<pre><code class="lang-php">&lt;?php
declare(ticks=1);
// some statements
declare(ticks=2);
// some statements
</code></pre>
</dd>
</dl>

<a name="Declare"></a>

## Declare ⇐ <code>Block</code>
**Kind**: global class  
**Extends**: <code>Block</code>  
**See**: http://php.net/manual/en/control-structures.declare.php  
**Properties**

| Name | Type |
| --- | --- |
| directives | <code>Array.&lt;Array&gt;</code> | 
| mode | <code>String</code> | 

<a name="MODE_SHORT"></a>

## MODE\_SHORT : <code>String</code>
The node is declared as a short tag syntax :
```php
<?php
declare(ticks=1):
// some statements
enddeclare;
```

**Kind**: global constant  
<a name="MODE_BLOCK"></a>

## MODE\_BLOCK : <code>String</code>
The node is declared bracket enclosed code :
```php
<?php
declare(ticks=1) {
// some statements
}
```

**Kind**: global constant  
<a name="MODE_NONE"></a>

## MODE\_NONE : <code>String</code>
The node is declared as a simple statement. In order to make things simpler
children of the node are automatically collected until the next
declare statement.
```php
<?php
declare(ticks=1);
// some statements
declare(ticks=2);
// some statements
```

**Kind**: global constant  
