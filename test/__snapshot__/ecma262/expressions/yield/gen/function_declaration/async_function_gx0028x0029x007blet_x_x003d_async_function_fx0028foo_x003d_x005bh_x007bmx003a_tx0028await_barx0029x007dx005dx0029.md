# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/yield/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/yield/gen/function_declaration
> :: test: function declaration
> :: case: async function g(){let x = async function f(foo = [h, {m: t(await bar)}]){}    }
## Options

`````js
{}
`````
## Input

`````js
function not_gen() { async function g(){let x = async function f(foo = [h, {m: t(await bar)}]){}    } }}
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
                                "text": "g",
                                "rawText": "g",
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
                                            "kind": 162,
                                            "lexicalKeyword": {
                                                "kind": 41951307,
                                                "flags": 80,
                                                "transformFlags": 0,
                                                "start": 40,
                                                "end": 43
                                            },
                                            "binding": {
                                                "kind": 151,
                                                "bindingList": [
                                                    {
                                                        "kind": 190,
                                                        "binding": {
                                                            "kind": 134299649,
                                                            "text": "x",
                                                            "rawText": "x",
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 43,
                                                            "end": 45
                                                        },
                                                        "type": null,
                                                        "initializer": {
                                                            "kind": 177,
                                                            "asyncKeyword": {
                                                                "kind": 82031,
                                                                "flags": 64,
                                                                "transformFlags": 0,
                                                                "start": 47,
                                                                "end": 53
                                                            },
                                                            "functionKeyword": {
                                                                "kind": 37822554,
                                                                "flags": 64,
                                                                "transformFlags": 0,
                                                                "start": 53,
                                                                "end": 62
                                                            },
                                                            "asteriskToken": null,
                                                            "name": {
                                                                "kind": 134299649,
                                                                "text": "f",
                                                                "rawText": "f",
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 62,
                                                                "end": 64
                                                            },
                                                            "typeParameters": null,
                                                            "formalParameterList": {
                                                                "kind": 214,
                                                                "formalParameters": [
                                                                    {
                                                                        "kind": 281,
                                                                        "ellipsisToken": null,
                                                                        "left": {
                                                                            "kind": 134299649,
                                                                            "text": "foo",
                                                                            "rawText": "foo",
                                                                            "flags": 96,
                                                                            "transformFlags": 0,
                                                                            "start": 65,
                                                                            "end": 68
                                                                        },
                                                                        "optionalToken": null,
                                                                        "type": null,
                                                                        "right": {
                                                                            "kind": 119,
                                                                            "elementList": {
                                                                                "kind": 270,
                                                                                "elements": [
                                                                                    {
                                                                                        "kind": 134299649,
                                                                                        "text": "h",
                                                                                        "rawText": "h",
                                                                                        "flags": 96,
                                                                                        "transformFlags": 0,
                                                                                        "start": 72,
                                                                                        "end": 73
                                                                                    },
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
                                                                                                        "start": 76,
                                                                                                        "end": 77
                                                                                                    },
                                                                                                    "right": {
                                                                                                        "kind": 131,
                                                                                                        "expression": {
                                                                                                            "kind": 134299649,
                                                                                                            "text": "t",
                                                                                                            "rawText": "t",
                                                                                                            "flags": 96,
                                                                                                            "transformFlags": 0,
                                                                                                            "start": 78,
                                                                                                            "end": 80
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
                                                                                                                        "start": 81,
                                                                                                                        "end": 86
                                                                                                                    },
                                                                                                                    "expression": {
                                                                                                                        "kind": 134299649,
                                                                                                                        "text": "bar",
                                                                                                                        "rawText": "bar",
                                                                                                                        "flags": 96,
                                                                                                                        "transformFlags": 0,
                                                                                                                        "start": 86,
                                                                                                                        "end": 90
                                                                                                                    },
                                                                                                                    "flags": 32,
                                                                                                                    "transformFlags": 4096,
                                                                                                                    "start": 81,
                                                                                                                    "end": 90
                                                                                                                }
                                                                                                            ],
                                                                                                            "trailingComma": false,
                                                                                                            "flags": 32,
                                                                                                            "transformFlags": 0,
                                                                                                            "start": 81,
                                                                                                            "end": 90
                                                                                                        },
                                                                                                        "flags": 32,
                                                                                                        "transformFlags": 1,
                                                                                                        "start": 76,
                                                                                                        "end": 91
                                                                                                    },
                                                                                                    "flags": 32,
                                                                                                    "transformFlags": 128,
                                                                                                    "start": 76,
                                                                                                    "end": 91
                                                                                                }
                                                                                            ],
                                                                                            "trailingComma": false,
                                                                                            "flags": 16,
                                                                                            "transformFlags": 0,
                                                                                            "start": 76,
                                                                                            "end": 91
                                                                                        },
                                                                                        "flags": 48,
                                                                                        "transformFlags": 8,
                                                                                        "start": 74,
                                                                                        "end": 92
                                                                                    }
                                                                                ],
                                                                                "trailingComma": false,
                                                                                "flags": 32,
                                                                                "transformFlags": 0,
                                                                                "start": 72,
                                                                                "end": 92
                                                                            },
                                                                            "flags": 32,
                                                                            "transformFlags": 8,
                                                                            "start": 70,
                                                                            "end": 93
                                                                        },
                                                                        "flags": 34,
                                                                        "transformFlags": 4096,
                                                                        "start": 65,
                                                                        "end": 93
                                                                    }
                                                                ],
                                                                "trailingComma": false,
                                                                "flags": 34,
                                                                "transformFlags": 0,
                                                                "start": 65,
                                                                "end": 93
                                                            },
                                                            "contents": {
                                                                "kind": 216,
                                                                "functionStatementList": {
                                                                    "kind": 217,
                                                                    "directives": [],
                                                                    "statements": [],
                                                                    "flags": 32,
                                                                    "transformFlags": 0,
                                                                    "start": 95,
                                                                    "end": 95
                                                                },
                                                                "flags": 32,
                                                                "transformFlags": 0,
                                                                "start": 94,
                                                                "end": 96
                                                            },
                                                            "returnType": null,
                                                            "flags": 160,
                                                            "transformFlags": 0,
                                                            "start": 47,
                                                            "end": 96
                                                        },
                                                        "flags": 16,
                                                        "transformFlags": 4224,
                                                        "start": 43,
                                                        "end": 96
                                                    }
                                                ],
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 43,
                                                "end": 96
                                            },
                                            "flags": 33554448,
                                            "transformFlags": 0,
                                            "start": 40,
                                            "end": 96
                                        }
                                    ],
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 40,
                                    "end": 96
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 39,
                                "end": 101
                            },
                            "returnType": null,
                            "flags": 144,
                            "transformFlags": 0,
                            "start": 20,
                            "end": 101
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 20,
                    "end": 101
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 18,
                "end": 103
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 103
        }
    ],
    "isModule": false,
    "source": "function not_gen() { async function g(){let x = async function f(foo = [h, {m: t(await bar)}]){}    } }}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 104
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ `await` expression cannot be used in function parameters - start: 81, end: 86
✖ Declaration or statement expected - start: 103, end: 104

```

