# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/yield/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/yield/gen/function_generator
> :: test: function generator
> :: case: async function a(){     async ([y] = [{m: 5 + t(await bar)}]) => {}     }
## Options

`````js
{}
`````
## Input

`````js
function * gen() { function not_gen() { async function a(){     async ([y] = [{m: 5 + t(await bar)}]) => {}     } }}
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 0,
                "end": 8
            },
            "asteriskToken": {
                "kind": 201360950,
                "flags": 64,
                "transformFlags": 32,
                "start": 8,
                "end": 10
            },
            "name": {
                "kind": 134299649,
                "text": "gen",
                "rawText": "gen",
                "flags": 96,
                "transformFlags": 0,
                "start": 10,
                "end": 14
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 15,
                "end": 15
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
                            "asyncKeyword": null,
                            "functionKeyword": {
                                "kind": 37822554,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 18,
                                "end": 27
                            },
                            "asteriskToken": null,
                            "name": {
                                "kind": 134299649,
                                "text": "not_gen",
                                "rawText": "not_gen",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 27,
                                "end": 35
                            },
                            "typeParameters": null,
                            "formalParameterList": {
                                "kind": 214,
                                "formalParameters": [],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 36,
                                "end": 36
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
                                                "start": 39,
                                                "end": 45
                                            },
                                            "functionKeyword": {
                                                "kind": 37822554,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 45,
                                                "end": 54
                                            },
                                            "asteriskToken": null,
                                            "name": {
                                                "kind": 134299649,
                                                "text": "a",
                                                "rawText": "a",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 54,
                                                "end": 56
                                            },
                                            "typeParameters": null,
                                            "formalParameterList": {
                                                "kind": 214,
                                                "formalParameters": [],
                                                "trailingComma": false,
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 57,
                                                "end": 57
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
                                                                    "start": 59,
                                                                    "end": 69
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
                                                                                            "start": 72,
                                                                                            "end": 73
                                                                                        }
                                                                                    ],
                                                                                    "trailingComma": false,
                                                                                    "flags": 32,
                                                                                    "transformFlags": 0,
                                                                                    "start": 72,
                                                                                    "end": 73
                                                                                },
                                                                                "flags": 32,
                                                                                "transformFlags": 0,
                                                                                "start": 71,
                                                                                "end": 74
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
                                                                                                            "start": 79,
                                                                                                            "end": 80
                                                                                                        },
                                                                                                        "right": {
                                                                                                            "kind": 198,
                                                                                                            "left": {
                                                                                                                "kind": 201392130,
                                                                                                                "text": 5,
                                                                                                                "rawText": "5",
                                                                                                                "flags": 96,
                                                                                                                "transformFlags": 0,
                                                                                                                "start": 81,
                                                                                                                "end": 83
                                                                                                            },
                                                                                                            "operatorToken": {
                                                                                                                "kind": 99634,
                                                                                                                "flags": 96,
                                                                                                                "transformFlags": 0,
                                                                                                                "start": 83,
                                                                                                                "end": 85
                                                                                                            },
                                                                                                            "right": {
                                                                                                                "kind": 131,
                                                                                                                "expression": {
                                                                                                                    "kind": 134299649,
                                                                                                                    "text": "t",
                                                                                                                    "rawText": "t",
                                                                                                                    "flags": 96,
                                                                                                                    "transformFlags": 0,
                                                                                                                    "start": 85,
                                                                                                                    "end": 87
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
                                                                                                                                "start": 88,
                                                                                                                                "end": 93
                                                                                                                            },
                                                                                                                            "expression": {
                                                                                                                                "kind": 134299649,
                                                                                                                                "text": "bar",
                                                                                                                                "rawText": "bar",
                                                                                                                                "flags": 96,
                                                                                                                                "transformFlags": 0,
                                                                                                                                "start": 93,
                                                                                                                                "end": 97
                                                                                                                            },
                                                                                                                            "flags": 32,
                                                                                                                            "transformFlags": 4096,
                                                                                                                            "start": 88,
                                                                                                                            "end": 97
                                                                                                                        }
                                                                                                                    ],
                                                                                                                    "trailingComma": false,
                                                                                                                    "flags": 32,
                                                                                                                    "transformFlags": 0,
                                                                                                                    "start": 88,
                                                                                                                    "end": 97
                                                                                                                },
                                                                                                                "flags": 32,
                                                                                                                "transformFlags": 1,
                                                                                                                "start": 85,
                                                                                                                "end": 98
                                                                                                            },
                                                                                                            "flags": 96,
                                                                                                            "transformFlags": 5120,
                                                                                                            "start": 79,
                                                                                                            "end": 98
                                                                                                        },
                                                                                                        "flags": 32,
                                                                                                        "transformFlags": 128,
                                                                                                        "start": 79,
                                                                                                        "end": 98
                                                                                                    }
                                                                                                ],
                                                                                                "trailingComma": false,
                                                                                                "flags": 16,
                                                                                                "transformFlags": 0,
                                                                                                "start": 79,
                                                                                                "end": 98
                                                                                            },
                                                                                            "flags": 48,
                                                                                            "transformFlags": 8,
                                                                                            "start": 78,
                                                                                            "end": 99
                                                                                        }
                                                                                    ],
                                                                                    "trailingComma": false,
                                                                                    "flags": 32,
                                                                                    "transformFlags": 0,
                                                                                    "start": 78,
                                                                                    "end": 99
                                                                                },
                                                                                "flags": 32,
                                                                                "transformFlags": 8,
                                                                                "start": 76,
                                                                                "end": 100
                                                                            },
                                                                            "flags": 32,
                                                                            "transformFlags": 4096,
                                                                            "start": 71,
                                                                            "end": 100
                                                                        }
                                                                    ],
                                                                    "trailingComma": false,
                                                                    "flags": 34,
                                                                    "transformFlags": 0,
                                                                    "start": 71,
                                                                    "end": 101
                                                                },
                                                                "returnType": null,
                                                                "arrowToken": {
                                                                    "kind": 10,
                                                                    "flags": 64,
                                                                    "transformFlags": 0,
                                                                    "start": 101,
                                                                    "end": 104
                                                                },
                                                                "contents": {
                                                                    "kind": 216,
                                                                    "functionStatementList": {
                                                                        "kind": 217,
                                                                        "directives": [],
                                                                        "statements": [],
                                                                        "flags": 32,
                                                                        "transformFlags": 0,
                                                                        "start": 106,
                                                                        "end": 106
                                                                    },
                                                                    "flags": 32,
                                                                    "transformFlags": 0,
                                                                    "start": 104,
                                                                    "end": 107
                                                                },
                                                                "flags": 290,
                                                                "transformFlags": 0,
                                                                "start": 59,
                                                                "end": 107
                                                            },
                                                            "flags": 16,
                                                            "transformFlags": 4096,
                                                            "start": 59,
                                                            "end": 107
                                                        }
                                                    ],
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 59,
                                                    "end": 107
                                                },
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 58,
                                                "end": 113
                                            },
                                            "returnType": null,
                                            "flags": 144,
                                            "transformFlags": 0,
                                            "start": 39,
                                            "end": 113
                                        }
                                    ],
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 39,
                                    "end": 113
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 37,
                                "end": 115
                            },
                            "returnType": null,
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 18,
                            "end": 115
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 18,
                    "end": 115
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 16,
                "end": 116
            },
            "returnType": null,
            "flags": 272,
            "transformFlags": 0,
            "start": 0,
            "end": 116
        }
    ],
    "isModule": false,
    "source": "function * gen() { function not_gen() { async function a(){     async ([y] = [{m: 5 + t(await bar)}]) => {}     } }}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 116
}
```

### Printed

```javascript
function *gen() {
  function not_gen() {
    async function a() {
      async ([y] = [{ m: 5 + t(await bar) }]) => {};
    }
  }
}
```

### Diagnostics

```javascript
✔ No errors
```

