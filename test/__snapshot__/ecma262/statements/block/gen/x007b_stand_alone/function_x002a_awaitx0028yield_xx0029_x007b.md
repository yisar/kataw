# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/block/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/block/gen/x007b_stand_alone
> :: test: { stand alone
> :: case: function * await(yield x) ; {
## Options

`````js
{}
`````
## Input

`````js
{ function * await(yield x) ; {
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
                        "kind": 176,
                        "declareKeyword": null,
                        "asyncKeyword": null,
                        "functionKeyword": {
                            "kind": 37822554,
                            "flags": 64,
                            "transformFlags": 0,
                            "start": 1,
                            "end": 10
                        },
                        "asteriskToken": {
                            "kind": 201360950,
                            "flags": 64,
                            "transformFlags": 32,
                            "start": 10,
                            "end": 12
                        },
                        "name": {
                            "kind": 134299649,
                            "text": "await",
                            "rawText": "await",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 12,
                            "end": 18
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
                                    "start": 19,
                                    "end": 24
                                },
                                {
                                    "kind": 134299649,
                                    "text": "x",
                                    "rawText": "x",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 24,
                                    "end": 26
                                }
                            ],
                            "trailingComma": false,
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 19,
                            "end": 26
                        },
                        "contents": {
                            "kind": 216,
                            "functionStatementList": {
                                "kind": 217,
                                "directives": [],
                                "statements": [],
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 27,
                                "end": 27
                            },
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 27,
                            "end": 27
                        },
                        "returnType": null,
                        "flags": 272,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 27
                    },
                    {
                        "kind": 168,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 27,
                        "end": 29
                    },
                    {
                        "kind": 124,
                        "block": {
                            "kind": 249,
                            "statements": [],
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 31,
                            "end": 31
                        },
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 29,
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
    "source": "{ function * await(yield x) ; {",
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
✖ `yield` expression cannot be used in function parameters - start: 19, end: 24
✖ ',' expected - start: 25, end: 26
✖ Missing an opening brace - '{ - start: 28, end: 29
✖ The parser expected to find a '}' to match the '{' token here - start: 30, end: 31

```

