# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/yield/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/yield/gen/function_declaration
> :: test: function declaration
> :: case: async function a(){     async ([y] = [{m: 5 + t(await bar)}]) => {}     }
## Options

`````js
{}
`````
## Input

`````js
function not_gen() { async function a(){     async ([y] = [{m: 5 + t(await bar)}]) => {}     } }}
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
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "not_gen",
                "rawText": "not_gen",
                "flags": 96,
                "transformFlags": 0,
                "start": 8,
                "end": 16
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 17,
                "end": 17
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
                                "start": 20,
                                "end": 26
                            },
                            "functionKeyword": {
                                "kind": 37822554,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 26,
                                "end": 35
                            },
                            "asteriskToken": null,
                            "name": {
                                "kind": 134299649,
                                "text": "a",
                                "rawText": "a",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 35,
                                "end": 37
                            },
                            "typeParameters": null,
                            "formalParameterList": {
                                "kind": 214,
                                "formalParameters": [],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 38,
                                "end": 38
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
                                                    "start": 40,
                                                    "end": 50
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
                                                                            "start": 53,
                                                                            "end": 54
                                                                        }
                                                                    ],
                                                                    "trailingComma": false,
                                                                    "flags": 32,
                                                                    "transformFlags": 0,
                                                                    "start": 53,
                                                                    "end": 54
                                                                },
                                                                "flags": 32,
                                                                "transformFlags": 0,
                                                                "start": 52,
                                                                "end": 55
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
                                                                                            "start": 60,
                                                                                            "end": 61
                                                                                        },
                                                                                        "right": {
                                                                                            "kind": 198,
                                                                                            "left": {
                                                                                                "kind": 201392130,
                                                                                                "text": 5,
                                                                                                "rawText": "5",
                                                                                                "flags": 96,
                                                                                                "transformFlags": 0,
                                                                                                "start": 62,
                                                                                                "end": 64
                                                                                            },
                                                                                            "operatorToken": {
                                                                                                "kind": 99634,
                                                                                                "flags": 96,
                                                                                                "transformFlags": 0,
                                                                                                "start": 64,
                                                                                                "end": 66
                                                                                            },
                                                                                            "right": {
                                                                                                "kind": 131,
                                                                                                "expression": {
                                                                                                    "kind": 134299649,
                                                                                                    "text": "t",
                                                                                                    "rawText": "t",
                                                                                                    "flags": 96,
                                                                                                    "transformFlags": 0,
                                                                                                    "start": 66,
                                                                                                    "end": 68
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
                                                                                                                "start": 69,
                                                                                                                "end": 74
                                                                                                            },
                                                                                                            "expression": {
                                                                                                                "kind": 134299649,
                                                                                                                "text": "bar",
                                                                                                                "rawText": "bar",
                                                                                                                "flags": 96,
                                                                                                                "transformFlags": 0,
                                                                                                                "start": 74,
                                                                                                                "end": 78
                                                                                                            },
                                                                                                            "flags": 32,
                                                                                                            "transformFlags": 4096,
                                                                                                            "start": 69,
                                                                                                            "end": 78
                                                                                                        }
                                                                                                    ],
                                                                                                    "trailingComma": false,
                                                                                                    "flags": 32,
                                                                                                    "transformFlags": 0,
                                                                                                    "start": 69,
                                                                                                    "end": 78
                                                                                                },
                                                                                                "flags": 32,
                                                                                                "transformFlags": 1,
                                                                                                "start": 66,
                                                                                                "end": 79
                                                                                            },
                                                                                            "flags": 96,
                                                                                            "transformFlags": 5120,
                                                                                            "start": 60,
                                                                                            "end": 79
                                                                                        },
                                                                                        "flags": 32,
                                                                                        "transformFlags": 128,
                                                                                        "start": 60,
                                                                                        "end": 79
                                                                                    }
                                                                                ],
                                                                                "trailingComma": false,
                                                                                "flags": 16,
                                                                                "transformFlags": 0,
                                                                                "start": 60,
                                                                                "end": 79
                                                                            },
                                                                            "flags": 48,
                                                                            "transformFlags": 8,
                                                                            "start": 59,
                                                                            "end": 80
                                                                        }
                                                                    ],
                                                                    "trailingComma": false,
                                                                    "flags": 32,
                                                                    "transformFlags": 0,
                                                                    "start": 59,
                                                                    "end": 80
                                                                },
                                                                "flags": 32,
                                                                "transformFlags": 8,
                                                                "start": 57,
                                                                "end": 81
                                                            },
                                                            "flags": 32,
                                                            "transformFlags": 4096,
                                                            "start": 52,
                                                            "end": 81
                                                        }
                                                    ],
                                                    "trailingComma": false,
                                                    "flags": 34,
                                                    "transformFlags": 0,
                                                    "start": 52,
                                                    "end": 82
                                                },
                                                "returnType": null,
                                                "arrowToken": {
                                                    "kind": 10,
                                                    "flags": 64,
                                                    "transformFlags": 0,
                                                    "start": 82,
                                                    "end": 85
                                                },
                                                "contents": {
                                                    "kind": 216,
                                                    "functionStatementList": {
                                                        "kind": 217,
                                                        "directives": [],
                                                        "statements": [],
                                                        "flags": 32,
                                                        "transformFlags": 0,
                                                        "start": 87,
                                                        "end": 87
                                                    },
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 85,
                                                    "end": 88
                                                },
                                                "flags": 290,
                                                "transformFlags": 0,
                                                "start": 40,
                                                "end": 88
                                            },
                                            "flags": 16,
                                            "transformFlags": 4096,
                                            "start": 40,
                                            "end": 88
                                        }
                                    ],
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 40,
                                    "end": 88
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 39,
                                "end": 94
                            },
                            "returnType": null,
                            "flags": 144,
                            "transformFlags": 0,
                            "start": 20,
                            "end": 94
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 20,
                    "end": 94
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 18,
                "end": 96
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 96
        }
    ],
    "isModule": false,
    "source": "function not_gen() { async function a(){     async ([y] = [{m: 5 + t(await bar)}]) => {}     } }}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 97
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Declaration or statement expected - start: 96, end: 97

```

