# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/yield/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/yield/gen/with_strict_dirctive
> :: test: with_strict_dirctive
> :: case: yield * 1; return 37; yield * 'dead';
## Options

`````js
{}
`````
## Input

`````js
'use strict'; yield * 1; return 37; yield * 'dead';
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [
        {
            "kind": 201392131,
            "text": "use strict",
            "rawText": "'use strict'",
            "flags": 4194400,
            "transformFlags": 0,
            "start": 0,
            "end": 12
        }
    ],
    "statements": [
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "yield",
                    "rawText": "yield",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 13,
                    "end": 19
                },
                "operatorToken": {
                    "kind": 201360950,
                    "flags": 96,
                    "transformFlags": 32,
                    "start": 19,
                    "end": 21
                },
                "right": {
                    "kind": 201392130,
                    "text": 1,
                    "rawText": "1",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 21,
                    "end": 23
                },
                "flags": 96,
                "transformFlags": 5120,
                "start": 13,
                "end": 23
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 13,
            "end": 24
        },
        {
            "kind": 161,
            "returnKeyword": {
                "kind": 37757022,
                "flags": 80,
                "transformFlags": 0,
                "start": 24,
                "end": 31
            },
            "expression": {
                "kind": 201392130,
                "text": 37,
                "rawText": "37",
                "flags": 96,
                "transformFlags": 0,
                "start": 31,
                "end": 34
            },
            "flags": 80,
            "transformFlags": 256,
            "start": 24,
            "end": 35
        },
        {
            "kind": 120,
            "expression": {
                "kind": 198,
                "left": {
                    "kind": 134299649,
                    "text": "yield",
                    "rawText": "yield",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 35,
                    "end": 41
                },
                "operatorToken": {
                    "kind": 201360950,
                    "flags": 96,
                    "transformFlags": 32,
                    "start": 41,
                    "end": 43
                },
                "right": {
                    "kind": 201392131,
                    "text": "dead",
                    "rawText": "'dead'",
                    "flags": 4194400,
                    "transformFlags": 0,
                    "start": 43,
                    "end": 50
                },
                "flags": 96,
                "transformFlags": 5120,
                "start": 35,
                "end": 50
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 35,
            "end": 51
        }
    ],
    "isModule": false,
    "source": "'use strict'; yield * 1; return 37; yield * 'dead';",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 51
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ A return statement can only be used within a function_body - start: 24, end: 31

```

