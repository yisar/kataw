# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/do-while/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/do-while/gen/do_with_unclosed_block
> :: test: do with unclosed block
> :: case: /**/ /x do while
## Options

`````js
{}
`````
## Input

`````js
do {} while (x) { /**/ /x do while
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
                "kind": 124,
                "block": {
                    "kind": 249,
                    "statements": [],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 4,
                    "end": 4
                },
                "flags": 16,
                "transformFlags": 0,
                "start": 2,
                "end": 5
            },
            "whileKeyword": {
                "kind": 37757028,
                "flags": 80,
                "transformFlags": 0,
                "start": 5,
                "end": 11
            },
            "expression": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 13,
                "end": 14
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 15
        },
        {
            "kind": 124,
            "block": {
                "kind": 249,
                "statements": [
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 371,
                            "text": "/x do while",
                            "rawText": "/x do while",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 17,
                            "end": 34
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 17,
                        "end": 34
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 17,
                "end": 34
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 15,
            "end": 34
        }
    ],
    "isModule": false,
    "source": "do {} while (x) { /**/ /x do while",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 34
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Unterminated regular expression - start: 17, end: 34
✖ The parser expected to find a '}' to match the '{' token here - start: 23, end: 34

```

