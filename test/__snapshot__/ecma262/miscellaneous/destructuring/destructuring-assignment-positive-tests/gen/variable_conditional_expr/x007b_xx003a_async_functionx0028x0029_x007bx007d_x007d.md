# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/miscellaneous/destructuring/destructuring-assignment-positive-tests/autogen.md
- Path: kataw/test/__snapshot__/ecma262/miscellaneous/destructuring/destructuring-assignment-positive-tests/gen/variable_conditional_expr
> :: test: variable conditional expr
> :: case: { x: async function() {} }
## Options

`````js
{}
`````
## Input

`````js
var x, y, z; m(['b']) ? lhs : { x: async function() {} } = {}
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "x",
                            "rawText": "x",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 5
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 3,
                        "end": 5
                    },
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "y",
                            "rawText": "y",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 6,
                            "end": 8
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 6,
                        "end": 8
                    },
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "z",
                            "rawText": "z",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 9,
                            "end": 11
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 9,
                        "end": 11
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 11
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 12
        },
        {
            "kind": 120,
            "expression": {
                "kind": 197,
                "shortCircuit": {
                    "kind": 131,
                    "expression": {
                        "kind": 134299649,
                        "text": "m",
                        "rawText": "m",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 12,
                        "end": 14
                    },
                    "argumentList": {
                        "kind": 256,
                        "elements": [
                            {
                                "kind": 119,
                                "elementList": {
                                    "kind": 270,
                                    "elements": [
                                        {
                                            "kind": 201392131,
                                            "text": "b",
                                            "rawText": "'b'",
                                            "flags": 4194400,
                                            "transformFlags": 0,
                                            "start": 16,
                                            "end": 19
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 4194336,
                                    "transformFlags": 0,
                                    "start": 16,
                                    "end": 19
                                },
                                "flags": 32,
                                "transformFlags": 8,
                                "start": 15,
                                "end": 20
                            }
                        ],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 15,
                        "end": 20
                    },
                    "flags": 32,
                    "transformFlags": 1,
                    "start": 12,
                    "end": 21
                },
                "questionToken": {
                    "kind": 134217750,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 21,
                    "end": 23
                },
                "consequent": {
                    "kind": 134299649,
                    "text": "lhs",
                    "rawText": "lhs",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 23,
                    "end": 27
                },
                "colonToken": {
                    "kind": 21,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 27,
                    "end": 29
                },
                "alternate": {
                    "kind": 125,
                    "left": {
                        "kind": 220,
                        "propertyList": {
                            "kind": 218,
                            "properties": [
                                {
                                    "kind": 219,
                                    "asteriskToken": null,
                                    "left": {
                                        "kind": 134299649,
                                        "text": "x",
                                        "rawText": "x",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 31,
                                        "end": 33
                                    },
                                    "right": {
                                        "kind": 177,
                                        "asyncKeyword": {
                                            "kind": 82031,
                                            "flags": 64,
                                            "transformFlags": 0,
                                            "start": 34,
                                            "end": 40
                                        },
                                        "functionKeyword": {
                                            "kind": 37822554,
                                            "flags": 64,
                                            "transformFlags": 0,
                                            "start": 40,
                                            "end": 49
                                        },
                                        "asteriskToken": null,
                                        "name": null,
                                        "typeParameters": null,
                                        "formalParameterList": {
                                            "kind": 214,
                                            "formalParameters": [],
                                            "trailingComma": false,
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 50,
                                            "end": 50
                                        },
                                        "contents": {
                                            "kind": 216,
                                            "functionStatementList": {
                                                "kind": 217,
                                                "directives": [],
                                                "statements": [],
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 53,
                                                "end": 53
                                            },
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 51,
                                            "end": 54
                                        },
                                        "returnType": null,
                                        "flags": 160,
                                        "transformFlags": 0,
                                        "start": 34,
                                        "end": 54
                                    },
                                    "flags": 32,
                                    "transformFlags": 128,
                                    "start": 31,
                                    "end": 54
                                }
                            ],
                            "trailingComma": false,
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 31,
                            "end": 54
                        },
                        "flags": 48,
                        "transformFlags": 8,
                        "start": 29,
                        "end": 56
                    },
                    "operatorToken": {
                        "kind": 4125,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 56,
                        "end": 58
                    },
                    "right": {
                        "kind": 220,
                        "propertyList": {
                            "kind": 218,
                            "properties": [],
                            "trailingComma": false,
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 60,
                            "end": 60
                        },
                        "flags": 48,
                        "transformFlags": 8,
                        "start": 58,
                        "end": 61
                    },
                    "flags": 32,
                    "transformFlags": 128,
                    "start": 29,
                    "end": 61
                },
                "flags": 32,
                "transformFlags": 4096,
                "start": 12,
                "end": 61
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 12,
            "end": 61
        }
    ],
    "isModule": false,
    "source": "var x, y, z; m(['b']) ? lhs : { x: async function() {} } = {}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 61
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ The left-hand side must be a variable or a property access. - start: 29, end: 58

```

