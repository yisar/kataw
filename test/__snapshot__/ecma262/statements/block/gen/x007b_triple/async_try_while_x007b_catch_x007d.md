# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/block/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/block/gen/x007b_triple
> :: test: { triple
> :: case: async try while { catch }
## Options

`````js
{}
`````
## Input

`````js
{ { { async try while { catch }
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
                                                "kind": 120,
                                                "expression": {
                                                    "kind": 134299649,
                                                    "text": "async",
                                                    "rawText": "async",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 5,
                                                    "end": 11
                                                },
                                                "flags": 16,
                                                "transformFlags": 4096,
                                                "start": 5,
                                                "end": 11
                                            },
                                            {
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
                                            {
                                                "kind": 154,
                                                "whileKeyword": {
                                                    "kind": 37757028,
                                                    "flags": 80,
                                                    "transformFlags": 0,
                                                    "start": 15,
                                                    "end": 21
                                                },
                                                "expression": {
                                                    "kind": 220,
                                                    "propertyList": {
                                                        "kind": 218,
                                                        "properties": [
                                                            {
                                                                "kind": 134299649,
                                                                "text": "catch",
                                                                "rawText": "catch",
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 23,
                                                                "end": 29
                                                            }
                                                        ],
                                                        "trailingComma": false,
                                                        "flags": 16,
                                                        "transformFlags": 0,
                                                        "start": 23,
                                                        "end": 29
                                                    },
                                                    "flags": 48,
                                                    "transformFlags": 8,
                                                    "start": 21,
                                                    "end": 31
                                                },
                                                "statement": {
                                                    "kind": 120,
                                                    "expression": {
                                                        "kind": 16637,
                                                        "text": "",
                                                        "rawText": "",
                                                        "flags": 64,
                                                        "transformFlags": 0,
                                                        "start": 31,
                                                        "end": 31
                                                    },
                                                    "flags": 16,
                                                    "transformFlags": 4096,
                                                    "start": 31,
                                                    "end": 31
                                                },
                                                "flags": 80,
                                                "transformFlags": 0,
                                                "start": 15,
                                                "end": 31
                                            }
                                        ],
                                        "flags": 16,
                                        "transformFlags": 0,
                                        "start": 5,
                                        "end": 31
                                    },
                                    "flags": 16,
                                    "transformFlags": 0,
                                    "start": 3,
                                    "end": 31
                                }
                            ],
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 31
                        },
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 31
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 1,
                "end": 31
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 31
        }
    ],
    "isModule": false,
    "source": "{ { { async try while { catch }",
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
✖ 'try' is not allowed here. Did you mean ';'? - start: 11, end: 15
✖ 'catch' expected - start: 15, end: 21
✖ Missing an opening parentheses - '( - start: 22, end: 23
✖ Property definition expected. Did you mean to use a ':'? - start: 29, end: 31
✖ Declaration or statement expected - start: 30, end: 31

```

