# AST

You can see the AST as a DOM document, the source code of the program beeing
the graphical text output, and the DOM beeing a representation of it.

The main node is the program node, and it's structured like this :

```js
  {
    "kind": "program",
    "children": [
      // array of nodes
    ]
  }
```

## Nodes

Every node has a common structure enabling you to scan them and act accordingly. 

NOTE : This structure depends also on what options you enable.

```js
  {
    "kind": "node name",
    "loc": {
      ""
    },
    // the location node
    "loc": {
      "source": "original source code of the node",
      "start": {
        "line": 1, // 1 based
        "column": 0, // 0 based
        "offset": 0 // offset from the source code
      },
      "end": {
        // same structure as start
      }
    },
    "leadingComments": [
      // array of comments nodes
    ]
  }
```

## Nodes hierarchy

 - [Location](#location)
 - [Position](#position)
 - [Node](#node)
   - [Identifier](#identifier)
   - [TraitUse](#traituse)
   - [TraitAlias](#traitalias)
   - [TraitPrecedence](#traitprecedence)
   - [Entry](#entry)
   - [Case](#case)
   - [Label](#label)
   - [Comment](#comment)
     - [CommentLine](#commentline)
     - [CommentBlock](#commentblock)
   - [Error](#error)
   - [Expression](#expression)
     - [Array](#array)
     - [Variable](#variable)
     - [Variadic](#variadic)
     - [ConstRef](#constref)
     - [Yield](#yield)
     - [YieldFrom](#yieldfrom)
     - [Lookup](#lookup)
       - [PropertyLookup](#propertylookup)
       - [StaticLookup](#staticlookup)
       - [OffsetLookup](#offsetlookup)
     - [Operation](#operation)
       - [Pre](#pre)
       - [Post](#post)
       - [Bin](#bin)
       - [Parenthesis](#parenthesis)
       - [Unary](#unary)
       - [Cast](#cast)
     - [Literal](#literal)
       - [Boolean](#boolean)
       - [String](#string)
       - [Number](#number)
       - [Inline](#inline)
       - [Magic](#magic)
       - [Nowdoc](#nowdoc)
       - [Encapsed](#encapsed)
   - [Statement](#statement)
     - [Eval](#eval)
     - [Exit](#exit)
     - [Halt](#halt)
     - [Clone](#clone)
     - [Declare](#declare)
     - [Global](#global)
     - [Static](#static)
     - [Include](#include)
     - [Assign](#assign)
     - [RetIf](#retif)
     - [If](#if)
     - [Do](#do)
     - [While](#while)
     - [For](#for)
     - [Foreach](#foreach)
     - [Switch](#switch)
     - [Goto](#goto)
     - [Silent](#silent)
     - [Try](#try)
     - [Catch](#catch)
     - [Throw](#throw)
     - [Call](#call)
     - [Closure](#closure)
     - [New](#new)
     - [UseGroup](#usegroup)
     - [UseItem](#useitem)
     - [Block](#block)
       - [Program](#program)
       - [Namespace](#namespace)
     - [Sys](#sys)
       - [Echo](#echo)
       - [List](#list)
       - [Print](#print)
       - [Isset](#isset)
       - [Unset](#unset)
       - [Empty](#empty)
     - [Declaration](#declaration)
       - [Class](#class)
       - [Interface](#interface)
       - [Trait](#trait)
       - [Constant](#constant)
         - [ClassConstant](#classconstant)
       - [Function](#function)
         - [Method](#method)
       - [Parameter](#parameter)
       - [Property](#property)

## AST
**Kind**: global class  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| withPositions | <code>Boolean</code> | Should locate any node (by default false) |
| withSource | <code>Boolean</code> | Should extract the node original code (by default false) |


* [AST](#AST)
    * [.swapLocations()](#AST+swapLocations)
    * [.resolvePrecedence()](#AST+resolvePrecedence)
    * [.prepare(kind, parser)](#AST+prepare) ⇒ <code>function</code>

<a name="AST+swapLocations"></a>

### asT.swapLocations()
Change parent node informations after swapping childs

**Kind**: instance method of [<code>AST</code>](#AST)  
<a name="AST+resolvePrecedence"></a>

### asT.resolvePrecedence()
Check and fix precence, by default using right

**Kind**: instance method of [<code>AST</code>](#AST)  
<a name="AST+prepare"></a>

### asT.prepare(kind, parser) ⇒ <code>function</code>
Prepares an AST node

**Kind**: instance method of [<code>AST</code>](#AST)  

| Param | Type | Description |
| --- | --- | --- |
| kind | <code>String</code> \| <code>null</code> | Defines the node type (if null, the kind must be passed at the function call) |
| parser | <code>Parser</code> | The parser instance (use for extracting locations) |

