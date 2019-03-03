## Classes

<dl>
<dt><a href="#Encapsed">Encapsed</a> ⇐ <code>Literal</code></dt>
<dd></dd>
</dl>

## Constants

<dl>
<dt><a href="#TYPE_STRING">TYPE_STRING</a> : <code>String</code></dt>
<dd><p>The node is a double quote string :</p>
<pre><code class="lang-php">&lt;?php
echo &quot;hello $world&quot;;
</code></pre>
</dd>
<dt><a href="#TYPE_SHELL">TYPE_SHELL</a> : <code>String</code></dt>
<dd><p>The node is a shell execute string :</p>
<pre><code class="lang-php">&lt;?php
echo `ls -larth $path`;
</code></pre>
</dd>
<dt><a href="#TYPE_HEREDOC">TYPE_HEREDOC</a> : <code>String</code></dt>
<dd><p>The node is a shell execute string :</p>
<pre><code class="lang-php">&lt;?php
echo &lt;&lt;&lt;STR
 Hello $world
STR
;
</code></pre>
</dd>
<dt><a href="#TYPE_OFFSET">TYPE_OFFSET</a> : <code>String</code></dt>
<dd><p>The node contains a list of constref / variables / expr :</p>
<pre><code class="lang-php">&lt;?php
echo $foo-&gt;bar_$baz;
</code></pre>
</dd>
</dl>

<a name="Encapsed"></a>

## Encapsed ⇐ <code>Literal</code>
**Kind**: global class  
**Extends**: <code>Literal</code>  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| type | <code>String</code> | Defines the type of encapsed string (shell, heredoc, string) |
| label | <code>String</code> \| <code>Null</code> | The heredoc label, defined only when the type is heredoc |

<a name="TYPE_STRING"></a>

## TYPE\_STRING : <code>String</code>
The node is a double quote string :
```php
<?php
echo "hello $world";
```

**Kind**: global constant  
<a name="TYPE_SHELL"></a>

## TYPE\_SHELL : <code>String</code>
The node is a shell execute string :
```php
<?php
echo `ls -larth $path`;
```

**Kind**: global constant  
<a name="TYPE_HEREDOC"></a>

## TYPE\_HEREDOC : <code>String</code>
The node is a shell execute string :
```php
<?php
echo <<<STR
 Hello $world
STR
;
```

**Kind**: global constant  
<a name="TYPE_OFFSET"></a>

## TYPE\_OFFSET : <code>String</code>
The node contains a list of constref / variables / expr :
```php
<?php
echo $foo->bar_$baz;
```

**Kind**: global constant  
