# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/classes/extends-lefthandside/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/classes/extends-lefthandside/gen/for-in_lhs
> :: test: for-in lhs
> :: case: -x
## Options

`````js
{}
`````
## Input

`````js
for (-x in x) ;
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 166,
            "forKeyword": {
                "kind": 37757017,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "initializer": {
                "kind": 126,
                "operandToken": {
                    "kind": 134318643,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 5,
                    "end": 6
                },
                "operand": {
                    "kind": 134299649,
                    "text": "x",
                    "rawText": "x",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 6,
                    "end": 7
                },
                "flags": 32,
                "transformFlags": 16384,
                "start": 5,
                "end": 7
            },
            "inKeyword": {
                "kind": 21006388,
                "flags": 64,
                "transformFlags": 0,
                "start": 7,
                "end": 10
            },
            "expression": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 10,
                "end": 12
            },
            "statement": {
                "kind": 168,
                "flags": 16,
                "transformFlags": 0,
                "start": 13,
                "end": 15
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 15
        }
    ],
    "isModule": false,
    "source": "for (-x in x) ;",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 15
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ The left-hand side of a 'for...in' statement must be a variable or a property access. - start: 10, end: 12

```

