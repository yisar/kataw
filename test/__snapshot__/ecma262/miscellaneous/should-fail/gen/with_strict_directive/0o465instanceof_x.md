# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/miscellaneous/should-fail/autogen.md
- Path: kataw/test/__snapshot__/ecma262/miscellaneous/should-fail/gen/with_strict_directive
> :: test: with strict directive
> :: case: 0o465instanceof x
## Options

`````js
{}
`````
## Input

`````js
"use strict"; 0o465instanceof x
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
                "kind": 201392130,
                "text": 309,
                "rawText": "0o465i",
                "flags": 262240,
                "transformFlags": 0,
                "start": 13,
                "end": 20
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 13,
            "end": 20
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "nstanceof",
                "rawText": "nstanceof",
                "flags": 96,
                "transformFlags": 0,
                "start": 20,
                "end": 29
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 20,
            "end": 29
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 29,
                "end": 31
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 29,
            "end": 31
        }
    ],
    "isModule": false,
    "source": "\"use strict\"; 0o465instanceof x",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 31
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ An identifier or keyword cannot immediately follow a numeric literal - start: 13, end: 19
✖ '; ' is not allowed here. Did you mean ';'? - start: 20, end: 29
✖ '; ' is not allowed here. Did you mean ';'? - start: 29, end: 31

```

