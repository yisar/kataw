# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/do-while/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/do-while/gen/with_unclosed_array
> :: test: with unclosed array
> :: case: catch try {}
## Options

`````js
{}
`````
## Input

`````js
do[ catch try {}
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
                    "kind": 119,
                    "elementList": {
                        "kind": 270,
                        "elements": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 3,
                        "end": 3
                    },
                    "flags": 32,
                    "transformFlags": 8,
                    "start": 2,
                    "end": 3
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 2,
                "end": 3
            },
            "whileKeyword": null,
            "expression": {
                "kind": 16637,
                "text": "",
                "rawText": "",
                "flags": 64,
                "transformFlags": 0,
                "start": 3,
                "end": 3
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 3
        },
        {
            "kind": 159,
            "tryKeyword": null,
            "block": {
                "kind": 124,
                "block": {
                    "kind": 249,
                    "statements": [],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 3,
                    "end": 3
                },
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 3
            },
            "catchClause": {
                "kind": 173,
                "catchKeyword": {
                    "kind": 4202575,
                    "flags": 80,
                    "transformFlags": 0,
                    "start": 3,
                    "end": 9
                },
                "catchParameter": null,
                "block": {
                    "kind": 124,
                    "block": {
                        "kind": 249,
                        "statements": [],
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 9,
                        "end": 9
                    },
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 9,
                    "end": 9
                },
                "flags": 80,
                "transformFlags": 0,
                "start": 3,
                "end": 9
            },
            "finallyKeyword": null,
            "finallyBlock": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 3,
            "end": 9
        },
        {
            "kind": 159,
            "tryKeyword": {
                "kind": 37757027,
                "flags": 80,
                "transformFlags": 0,
                "start": 9,
                "end": 13
            },
            "block": {
                "kind": 124,
                "block": {
                    "kind": 249,
                    "statements": [],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 15,
                    "end": 15
                },
                "flags": 16,
                "transformFlags": 0,
                "start": 13,
                "end": 16
            },
            "catchClause": null,
            "finallyKeyword": null,
            "finallyBlock": {
                "kind": 124,
                "block": {
                    "kind": 249,
                    "statements": [],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 16,
                    "end": 16
                },
                "flags": 16,
                "transformFlags": 0,
                "start": 16,
                "end": 16
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 9,
            "end": 16
        }
    ],
    "isModule": false,
    "source": "do[ catch try {}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 16
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Did you forgot a ']' to match the `[` token? - start: 4, end: 9
✖ 'catch' expected - start: 16, end: 16

```

