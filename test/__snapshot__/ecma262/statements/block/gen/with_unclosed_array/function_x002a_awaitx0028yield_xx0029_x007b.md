# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/block/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/block/gen/with_unclosed_array
> :: test: with unclosed array
> :: case: function * await(yield x) ; {
## Options

`````js
{}
`````
## Input

`````js
{[ function * await(yield x) ; {
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
                        "kind": 120,
                        "expression": {
                            "kind": 119,
                            "elementList": {
                                "kind": 270,
                                "elements": [
                                    {
                                        "kind": 177,
                                        "asyncKeyword": null,
                                        "functionKeyword": {
                                            "kind": 37822554,
                                            "flags": 64,
                                            "transformFlags": 0,
                                            "start": 2,
                                            "end": 11
                                        },
                                        "asteriskToken": {
                                            "kind": 201360950,
                                            "flags": 64,
                                            "transformFlags": 32,
                                            "start": 11,
                                            "end": 13
                                        },
                                        "name": {
                                            "kind": 134299649,
                                            "text": "await",
                                            "rawText": "await",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 13,
                                            "end": 19
                                        },
                                        "typeParameters": null,
                                        "formalParameterList": {
                                            "kind": 214,
                                            "formalParameters": [
                                                {
                                                    "kind": 134299649,
                                                    "text": "yield",
                                                    "rawText": "yield",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 20,
                                                    "end": 25
                                                },
                                                {
                                                    "kind": 134299649,
                                                    "text": "x",
                                                    "rawText": "x",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 25,
                                                    "end": 27
                                                }
                                            ],
                                            "trailingComma": false,
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 20,
                                            "end": 27
                                        },
                                        "contents": {
                                            "kind": 216,
                                            "functionStatementList": {
                                                "kind": 217,
                                                "directives": [],
                                                "statements": [],
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 28,
                                                "end": 28
                                            },
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 28,
                                            "end": 28
                                        },
                                        "returnType": null,
                                        "flags": 288,
                                        "transformFlags": 0,
                                        "start": 2,
                                        "end": 28
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 2,
                                "end": 28
                            },
                            "flags": 32,
                            "transformFlags": 8,
                            "start": 1,
                            "end": 28
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 1,
                        "end": 30
                    },
                    {
                        "kind": 124,
                        "block": {
                            "kind": 249,
                            "statements": [],
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 32,
                            "end": 32
                        },
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 30,
                        "end": 32
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 1,
                "end": 32
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 32
        }
    ],
    "isModule": false,
    "source": "{[ function * await(yield x) ; {",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 32
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ `yield` expression cannot be used in function parameters - start: 20, end: 25
✖ ',' expected - start: 26, end: 27
✖ Missing an opening brace - '{ - start: 29, end: 30
✖ The parser expected to find a '}' to match the '{' token here - start: 31, end: 32

```

