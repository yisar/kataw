# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/do-while/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/do-while/gen/do_triple
> :: test: do triple
> :: case: /**/ /x do while
## Options

`````js
{}
`````
## Input

`````js
do do do /**/ /x do while while while while
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
                "kind": 169,
                "doKeyword": {
                    "kind": 4202580,
                    "flags": 80,
                    "transformFlags": 0,
                    "start": 2,
                    "end": 5
                },
                "statement": {
                    "kind": 169,
                    "doKeyword": {
                        "kind": 4202580,
                        "flags": 80,
                        "transformFlags": 0,
                        "start": 5,
                        "end": 8
                    },
                    "statement": {
                        "kind": 120,
                        "expression": {
                            "kind": 371,
                            "text": "/x do while while while while",
                            "rawText": "/x do while while while while",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 8,
                            "end": 43
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 8,
                        "end": 43
                    },
                    "whileKeyword": null,
                    "expression": {
                        "kind": 16637,
                        "text": "",
                        "rawText": "",
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 43,
                        "end": 43
                    },
                    "flags": 80,
                    "transformFlags": 0,
                    "start": 5,
                    "end": 43
                },
                "whileKeyword": null,
                "expression": {
                    "kind": 16637,
                    "text": "",
                    "rawText": "",
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 43,
                    "end": 43
                },
                "flags": 80,
                "transformFlags": 0,
                "start": 2,
                "end": 43
            },
            "whileKeyword": null,
            "expression": {
                "kind": 16637,
                "text": "",
                "rawText": "",
                "flags": 64,
                "transformFlags": 0,
                "start": 43,
                "end": 43
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 43
        }
    ],
    "isModule": false,
    "source": "do do do /**/ /x do while while while while",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 43
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Unterminated regular expression - start: 8, end: 43
✖ Missing an opening parentheses - '( - start: 14, end: 43

```

