# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/await/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/await/gen/var
> :: test: var
> :: case: async function a(){     async ([y] = [{m: 5 + t(await bar)}]) => {}     }
## Options

`````js
{}
`````
## Input

`````js
var await; var f = (async function() { async function a(){     async ([y] = [{m: 5 + t(await bar)}]) => {}     } });
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
                            "text": "await",
                            "rawText": "await",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 9
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 3,
                        "end": 9
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 9
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 10
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 80,
                "transformFlags": 0,
                "start": 10,
                "end": 14
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "f",
                            "rawText": "f",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 14,
                            "end": 16
                        },
                        "type": null,
                        "initializer": {
                            "kind": 121,
                            "expression": {
                                "kind": 177,
                                "asyncKeyword": {
                                    "kind": 82031,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 20,
                                    "end": 25
                                },
                                "functionKeyword": {
                                    "kind": 37822554,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 25,
                                    "end": 34
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
                                    "start": 35,
                                    "end": 35
                                },
                                "contents": {
                                    "kind": 216,
                                    "functionStatementList": {
                                        "kind": 217,
                                        "directives": [],
                                        "statements": [
                                            {
                                                "kind": 176,
                                                "declareKeyword": null,
                                                "asyncKeyword": {
                                                    "kind": 82031,
                                                    "flags": 64,
                                                    "transformFlags": 0,
                                                    "start": 38,
                                                    "end": 44
                                                },
                                                "functionKeyword": {
                                                    "kind": 37822554,
                                                    "flags": 64,
                                                    "transformFlags": 0,
                                                    "start": 44,
                                                    "end": 53
                                                },
                                                "asteriskToken": null,
                                                "name": {
                                                    "kind": 134299649,
                                                    "text": "a",
                                                    "rawText": "a",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 53,
                                                    "end": 55
                                                },
                                                "typeParameters": null,
                                                "formalParameterList": {
                                                    "kind": 214,
                                                    "formalParameters": [],
                                                    "trailingComma": false,
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 56,
                                                    "end": 56
                                                },
                                                "contents": {
                                                    "kind": 216,
                                                    "functionStatementList": {
                                                        "kind": 217,
                                                        "directives": [],
                                                        "statements": [
                                                            {
                                                                "kind": 120,
                                                                "expression": {
                                                                    "kind": 271,
                                                                    "asyncKeyword": {
                                                                        "kind": 82031,
                                                                        "flags": 64,
                                                                        "transformFlags": 0,
                                                                        "start": 58,
                                                                        "end": 68
                                                                    },
                                                                    "typeParameters": null,
                                                                    "arrowPatameterList": {
                                                                        "kind": 342,
                                                                        "parameters": [
                                                                            {
                                                                                "kind": 281,
                                                                                "ellipsisToken": null,
                                                                                "left": {
                                                                                    "kind": 201,
                                                                                    "elementList": {
                                                                                        "kind": 270,
                                                                                        "elements": [
                                                                                            {
                                                                                                "kind": 134299649,
                                                                                                "text": "y",
                                                                                                "rawText": "y",
                                                                                                "flags": 96,
                                                                                                "transformFlags": 0,
                                                                                                "start": 71,
                                                                                                "end": 72
                                                                                            }
                                                                                        ],
                                                                                        "trailingComma": false,
                                                                                        "flags": 32,
                                                                                        "transformFlags": 0,
                                                                                        "start": 71,
                                                                                        "end": 72
                                                                                    },
                                                                                    "flags": 32,
                                                                                    "transformFlags": 0,
                                                                                    "start": 70,
                                                                                    "end": 73
                                                                                },
                                                                                "optionalToken": null,
                                                                                "type": null,
                                                                                "right": {
                                                                                    "kind": 119,
                                                                                    "elementList": {
                                                                                        "kind": 270,
                                                                                        "elements": [
                                                                                            {
                                                                                                "kind": 220,
                                                                                                "propertyList": {
                                                                                                    "kind": 218,
                                                                                                    "properties": [
                                                                                                        {
                                                                                                            "kind": 219,
                                                                                                            "asteriskToken": null,
                                                                                                            "left": {
                                                                                                                "kind": 134299649,
                                                                                                                "text": "m",
                                                                                                                "rawText": "m",
                                                                                                                "flags": 96,
                                                                                                                "transformFlags": 0,
                                                                                                                "start": 78,
                                                                                                                "end": 79
                                                                                                            },
                                                                                                            "right": {
                                                                                                                "kind": 198,
                                                                                                                "left": {
                                                                                                                    "kind": 201392130,
                                                                                                                    "text": 5,
                                                                                                                    "rawText": "5",
                                                                                                                    "flags": 96,
                                                                                                                    "transformFlags": 0,
                                                                                                                    "start": 80,
                                                                                                                    "end": 82
                                                                                                                },
                                                                                                                "operatorToken": {
                                                                                                                    "kind": 99634,
                                                                                                                    "flags": 96,
                                                                                                                    "transformFlags": 0,
                                                                                                                    "start": 82,
                                                                                                                    "end": 84
                                                                                                                },
                                                                                                                "right": {
                                                                                                                    "kind": 131,
                                                                                                                    "expression": {
                                                                                                                        "kind": 134299649,
                                                                                                                        "text": "t",
                                                                                                                        "rawText": "t",
                                                                                                                        "flags": 96,
                                                                                                                        "transformFlags": 0,
                                                                                                                        "start": 84,
                                                                                                                        "end": 86
                                                                                                                    },
                                                                                                                    "argumentList": {
                                                                                                                        "kind": 256,
                                                                                                                        "elements": [
                                                                                                                            {
                                                                                                                                "kind": 208,
                                                                                                                                "awaitKeyword": {
                                                                                                                                    "kind": 82196,
                                                                                                                                    "flags": 64,
                                                                                                                                    "transformFlags": 0,
                                                                                                                                    "start": 87,
                                                                                                                                    "end": 92
                                                                                                                                },
                                                                                                                                "expression": {
                                                                                                                                    "kind": 134299649,
                                                                                                                                    "text": "bar",
                                                                                                                                    "rawText": "bar",
                                                                                                                                    "flags": 96,
                                                                                                                                    "transformFlags": 0,
                                                                                                                                    "start": 92,
                                                                                                                                    "end": 96
                                                                                                                                },
                                                                                                                                "flags": 32,
                                                                                                                                "transformFlags": 4096,
                                                                                                                                "start": 87,
                                                                                                                                "end": 96
                                                                                                                            }
                                                                                                                        ],
                                                                                                                        "trailingComma": false,
                                                                                                                        "flags": 32,
                                                                                                                        "transformFlags": 0,
                                                                                                                        "start": 87,
                                                                                                                        "end": 96
                                                                                                                    },
                                                                                                                    "flags": 32,
                                                                                                                    "transformFlags": 1,
                                                                                                                    "start": 84,
                                                                                                                    "end": 97
                                                                                                                },
                                                                                                                "flags": 96,
                                                                                                                "transformFlags": 5120,
                                                                                                                "start": 78,
                                                                                                                "end": 97
                                                                                                            },
                                                                                                            "flags": 32,
                                                                                                            "transformFlags": 128,
                                                                                                            "start": 78,
                                                                                                            "end": 97
                                                                                                        }
                                                                                                    ],
                                                                                                    "trailingComma": false,
                                                                                                    "flags": 16,
                                                                                                    "transformFlags": 0,
                                                                                                    "start": 78,
                                                                                                    "end": 97
                                                                                                },
                                                                                                "flags": 48,
                                                                                                "transformFlags": 8,
                                                                                                "start": 77,
                                                                                                "end": 98
                                                                                            }
                                                                                        ],
                                                                                        "trailingComma": false,
                                                                                        "flags": 32,
                                                                                        "transformFlags": 0,
                                                                                        "start": 77,
                                                                                        "end": 98
                                                                                    },
                                                                                    "flags": 32,
                                                                                    "transformFlags": 8,
                                                                                    "start": 75,
                                                                                    "end": 99
                                                                                },
                                                                                "flags": 32,
                                                                                "transformFlags": 4096,
                                                                                "start": 70,
                                                                                "end": 99
                                                                            }
                                                                        ],
                                                                        "trailingComma": false,
                                                                        "flags": 34,
                                                                        "transformFlags": 0,
                                                                        "start": 70,
                                                                        "end": 100
                                                                    },
                                                                    "returnType": null,
                                                                    "arrowToken": {
                                                                        "kind": 10,
                                                                        "flags": 64,
                                                                        "transformFlags": 0,
                                                                        "start": 100,
                                                                        "end": 103
                                                                    },
                                                                    "contents": {
                                                                        "kind": 216,
                                                                        "functionStatementList": {
                                                                            "kind": 217,
                                                                            "directives": [],
                                                                            "statements": [],
                                                                            "flags": 32,
                                                                            "transformFlags": 0,
                                                                            "start": 105,
                                                                            "end": 105
                                                                        },
                                                                        "flags": 32,
                                                                        "transformFlags": 0,
                                                                        "start": 103,
                                                                        "end": 106
                                                                    },
                                                                    "flags": 290,
                                                                    "transformFlags": 0,
                                                                    "start": 58,
                                                                    "end": 106
                                                                },
                                                                "flags": 16,
                                                                "transformFlags": 4096,
                                                                "start": 58,
                                                                "end": 106
                                                            }
                                                        ],
                                                        "flags": 32,
                                                        "transformFlags": 0,
                                                        "start": 58,
                                                        "end": 106
                                                    },
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 57,
                                                    "end": 112
                                                },
                                                "returnType": null,
                                                "flags": 144,
                                                "transformFlags": 0,
                                                "start": 38,
                                                "end": 112
                                            }
                                        ],
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 38,
                                        "end": 112
                                    },
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 36,
                                    "end": 114
                                },
                                "returnType": null,
                                "flags": 160,
                                "transformFlags": 0,
                                "start": 20,
                                "end": 114
                            },
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 18,
                            "end": 115
                        },
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 14,
                        "end": 115
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 14,
                "end": 115
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 10,
            "end": 116
        }
    ],
    "isModule": false,
    "source": "var await; var f = (async function() { async function a(){     async ([y] = [{m: 5 + t(await bar)}]) => {}     } });",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 116
}
```

### Printed

```javascript
var await;
var f = (async function () {
    async function a() {
      async ([y] = [{ m: 5 + t(await bar) }]) => {};
    }
  });

```

### Diagnostics

```javascript
✔ No errors
```

