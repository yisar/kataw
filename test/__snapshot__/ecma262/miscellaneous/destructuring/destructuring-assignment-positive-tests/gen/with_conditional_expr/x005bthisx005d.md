# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/miscellaneous/destructuring/destructuring-assignment-positive-tests/autogen.md
- Path: kataw/test/__snapshot__/ecma262/miscellaneous/destructuring/destructuring-assignment-positive-tests/gen/with_conditional_expr
> :: test: with conditional expr
> :: case: [this]
## Options

`````js
{}
`````
## Input

`````js
'use strict'; var x, y, z; m(['a']) ? [this] = {} : rhs
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
            "rawText": "'use strict'",
            "flags": 4194400,
            "transformFlags": 0,
            "start": 0,
            "end": 12
        }
    ],
    "statements": [
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 80,
                "transformFlags": 0,
                "start": 13,
                "end": 17
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
                            "start": 17,
                            "end": 19
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 17,
                        "end": 19
                    },
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "y",
                            "rawText": "y",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 20,
                            "end": 22
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 20,
                        "end": 22
                    },
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "z",
                            "rawText": "z",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 23,
                            "end": 25
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 23,
                        "end": 25
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 17,
                "end": 25
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 13,
            "end": 26
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
                        "start": 26,
                        "end": 28
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
                                            "text": "a",
                                            "rawText": "'a'",
                                            "flags": 4194400,
                                            "transformFlags": 0,
                                            "start": 30,
                                            "end": 33
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 4194336,
                                    "transformFlags": 0,
                                    "start": 30,
                                    "end": 33
                                },
                                "flags": 32,
                                "transformFlags": 8,
                                "start": 29,
                                "end": 34
                            }
                        ],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 29,
                        "end": 34
                    },
                    "flags": 32,
                    "transformFlags": 1,
                    "start": 26,
                    "end": 35
                },
                "questionToken": {
                    "kind": 134217750,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 35,
                    "end": 37
                },
                "consequent": {
                    "kind": 125,
                    "left": {
                        "kind": 119,
                        "elementList": {
                            "kind": 270,
                            "elements": [
                                {
                                    "kind": 4276321,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 39,
                                    "end": 43
                                }
                            ],
                            "trailingComma": false,
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 39,
                            "end": 43
                        },
                        "flags": 32,
                        "transformFlags": 8,
                        "start": 37,
                        "end": 44
                    },
                    "operatorToken": {
                        "kind": 4125,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 44,
                        "end": 46
                    },
                    "right": {
                        "kind": 220,
                        "propertyList": {
                            "kind": 218,
                            "properties": [],
                            "trailingComma": false,
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 48,
                            "end": 48
                        },
                        "flags": 48,
                        "transformFlags": 8,
                        "start": 46,
                        "end": 49
                    },
                    "flags": 32,
                    "transformFlags": 128,
                    "start": 37,
                    "end": 49
                },
                "colonToken": {
                    "kind": 21,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 49,
                    "end": 51
                },
                "alternate": {
                    "kind": 134299649,
                    "text": "rhs",
                    "rawText": "rhs",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 51,
                    "end": 55
                },
                "flags": 32,
                "transformFlags": 4096,
                "start": 26,
                "end": 55
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 26,
            "end": 55
        }
    ],
    "isModule": false,
    "source": "'use strict'; var x, y, z; m(['a']) ? [this] = {} : rhs",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 55
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ The left-hand side must be a variable or a property access. - start: 44, end: 46

```

