# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/arrow/type-annotation/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/arrow/type-annotation/gen/strict_directive
> :: test: strict directive
> :: case: ({x: [y: string]}: string = y, z?) => ok
## Options

`````js
{}
`````
## Input

`````js
"use strict"; ({x: [y: string]}: string = y, z?) => ok
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
            "rawText": "\"use strict\"",
            "flags": 96,
            "transformFlags": 0,
            "start": 0,
            "end": 12
        }
    ],
    "statements": [
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 132,
                    "expressions": [],
                    "flags": 32,
                    "transformFlags": 1024,
                    "start": 13,
                    "end": 21
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 13,
                "end": 21
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 13,
            "end": 21
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "string",
                "rawText": "string",
                "flags": 96,
                "transformFlags": 0,
                "start": 22,
                "end": 29
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 22,
            "end": 29
        },
        {
            "kind": 120,
            "expression": {
                "kind": 132,
                "expressions": [
                    {
                        "kind": 125,
                        "left": {
                            "kind": 134299649,
                            "text": "string",
                            "rawText": "string",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 32,
                            "end": 39
                        },
                        "operatorToken": {
                            "kind": 4125,
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 39,
                            "end": 41
                        },
                        "right": {
                            "kind": 134299649,
                            "text": "y",
                            "rawText": "y",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 41,
                            "end": 43
                        },
                        "flags": 0,
                        "transformFlags": 128,
                        "start": 32,
                        "end": 43
                    },
                    {
                        "kind": 197,
                        "shortCircuit": {
                            "kind": 134299649,
                            "text": "z",
                            "rawText": "z",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 44,
                            "end": 46
                        },
                        "questionToken": {
                            "kind": 134217750,
                            "flags": 64,
                            "transformFlags": 0,
                            "start": 46,
                            "end": 47
                        },
                        "consequent": {
                            "kind": 16637,
                            "text": "",
                            "rawText": "",
                            "flags": 64,
                            "transformFlags": 0,
                            "start": 47,
                            "end": 47
                        },
                        "colonToken": null,
                        "alternate": {
                            "kind": 16637,
                            "text": "",
                            "rawText": "",
                            "flags": 64,
                            "transformFlags": 0,
                            "start": 47,
                            "end": 47
                        },
                        "flags": 96,
                        "transformFlags": 4096,
                        "start": 44,
                        "end": 47
                    }
                ],
                "flags": 32,
                "transformFlags": 1024,
                "start": 32,
                "end": 47
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 32,
            "end": 47
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "ok",
                "rawText": "ok",
                "flags": 96,
                "transformFlags": 0,
                "start": 51,
                "end": 54
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 51,
            "end": 54
        }
    ],
    "isModule": false,
    "source": "\"use strict\"; ({x: [y: string]}: string = y, z?) => ok",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 54
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ ',' expected - start: 21, end: 22
✖ ']' is not allowed here. Did you mean ';'? - start: 29, end: 30
✖ Declaration or statement expected - start: 30, end: 31
✖ Declaration or statement expected - start: 31, end: 32
✖ Identifier expected - start: 47, end: 48
✖ Declaration or statement expected - start: 48, end: 51

```

