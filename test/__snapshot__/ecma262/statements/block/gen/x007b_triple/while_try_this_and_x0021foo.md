# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/block/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/block/gen/x007b_triple
> :: test: { triple
> :: case: while try this and !foo
## Options

`````js
{}
`````
## Input

`````js
{ { { while try this and !foo
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 124,
            "block": {
                "kind": 249,
                "statements": [
                    {
                        "kind": 124,
                        "block": {
                            "kind": 249,
                            "statements": [
                                {
                                    "kind": 124,
                                    "block": {
                                        "kind": 249,
                                        "statements": [
                                            {
                                                "kind": 154,
                                                "whileKeyword": {
                                                    "kind": 37757028,
                                                    "flags": 80,
                                                    "transformFlags": 0,
                                                    "start": 5,
                                                    "end": 11
                                                },
                                                "expression": {
                                                    "kind": 16637,
                                                    "text": "",
                                                    "rawText": "",
                                                    "flags": 64,
                                                    "transformFlags": 0,
                                                    "start": 11,
                                                    "end": 11
                                                },
                                                "statement": {
                                                    "kind": 159,
                                                    "tryKeyword": {
                                                        "kind": 37757027,
                                                        "flags": 80,
                                                        "transformFlags": 0,
                                                        "start": 11,
                                                        "end": 15
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
                                                        "start": 15,
                                                        "end": 15
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
                                                            "start": 15,
                                                            "end": 15
                                                        },
                                                        "flags": 16,
                                                        "transformFlags": 0,
                                                        "start": 15,
                                                        "end": 15
                                                    },
                                                    "flags": 16,
                                                    "transformFlags": 0,
                                                    "start": 11,
                                                    "end": 15
                                                },
                                                "flags": 80,
                                                "transformFlags": 0,
                                                "start": 5,
                                                "end": 15
                                            },
                                            {
                                                "kind": 120,
                                                "expression": {
                                                    "kind": 4276321,
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 15,
                                                    "end": 20
                                                },
                                                "flags": 16,
                                                "transformFlags": 4096,
                                                "start": 15,
                                                "end": 20
                                            },
                                            {
                                                "kind": 120,
                                                "expression": {
                                                    "kind": 134299649,
                                                    "text": "and",
                                                    "rawText": "and",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 20,
                                                    "end": 24
                                                },
                                                "flags": 16,
                                                "transformFlags": 4096,
                                                "start": 20,
                                                "end": 24
                                            },
                                            {
                                                "kind": 120,
                                                "expression": {
                                                    "kind": 126,
                                                    "operandToken": {
                                                        "kind": 65584,
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 24,
                                                        "end": 26
                                                    },
                                                    "operand": {
                                                        "kind": 134299649,
                                                        "text": "foo",
                                                        "rawText": "foo",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 26,
                                                        "end": 29
                                                    },
                                                    "flags": 32,
                                                    "transformFlags": 16384,
                                                    "start": 24,
                                                    "end": 29
                                                },
                                                "flags": 16,
                                                "transformFlags": 4096,
                                                "start": 24,
                                                "end": 29
                                            }
                                        ],
                                        "flags": 16,
                                        "transformFlags": 0,
                                        "start": 5,
                                        "end": 29
                                    },
                                    "flags": 16,
                                    "transformFlags": 0,
                                    "start": 3,
                                    "end": 29
                                }
                            ],
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 29
                        },
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 29
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 1,
                "end": 29
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 29
        }
    ],
    "isModule": false,
    "source": "{ { { while try this and !foo",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 29
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Missing an opening parentheses - '( - start: 12, end: 15
✖ 'catch' expected - start: 15, end: 20
✖ '; ' is not allowed here. Did you mean ';'? - start: 20, end: 24
✖ '!' is not allowed here. Did you mean ';'? - start: 24, end: 26
✖ The parser expected to find a '}' to match the '{' token here - start: 26, end: 29

```

