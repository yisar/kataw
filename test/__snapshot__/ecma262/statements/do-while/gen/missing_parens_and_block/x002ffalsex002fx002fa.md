# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/do-while/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/do-while/gen/missing_parens_and_block
> :: test: missing parens and block
> :: case: /false//a
## Options

`````js
{}
`````
## Input

`````js
do /false//a while
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 169,
            "doKeyword": {
                "kind": 4202580,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 2
            },
            "statement": {
                "kind": 120,
                "expression": {
                    "kind": 198,
                    "left": {
                        "kind": 371,
                        "text": "/false/",
                        "rawText": "/false/",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 2,
                        "end": 10
                    },
                    "operatorToken": {
                        "kind": 35640,
                        "flags": 96,
                        "transformFlags": 32,
                        "start": 10,
                        "end": 11
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "a",
                        "rawText": "a",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 11,
                        "end": 12
                    },
                    "flags": 96,
                    "transformFlags": 5120,
                    "start": 2,
                    "end": 12
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 2,
                "end": 12
            },
            "whileKeyword": {
                "kind": 37757028,
                "flags": 80,
                "transformFlags": 0,
                "start": 12,
                "end": 18
            },
            "expression": {
                "kind": 16637,
                "text": "",
                "rawText": "",
                "flags": 64,
                "transformFlags": 0,
                "start": 18,
                "end": 18
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 18
        }
    ],
    "isModule": false,
    "source": "do /false//a while",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 18
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ 'while' is not allowed here. Did you mean ';'? - start: 12, end: 18

```

