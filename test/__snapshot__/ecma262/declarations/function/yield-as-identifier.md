# Kataw parser test case

## Input

`````js
function foo() { ({yield} = x) }

function foo() { let x = {yield} }

function *foo() { ({yield} = x) }

function *foo() { let x = {yield} }
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
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 8,
                "end": 12
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 13,
                "end": 13
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
                                "kind": 121,
                                "expression": {
                                    "kind": 125,
                                    "left": {
                                        "kind": 220,
                                        "propertyList": {
                                            "kind": 218,
                                            "properties": [
                                                {
                                                    "kind": 134299649,
                                                    "text": "yield",
                                                    "rawText": "yield",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 19,
                                                    "end": 24
                                                }
                                            ],
                                            "trailingComma": false,
                                            "flags": 16,
                                            "transformFlags": 0,
                                            "start": 19,
                                            "end": 24
                                        },
                                        "flags": 48,
                                        "transformFlags": 8,
                                        "start": 18,
                                        "end": 25
                                    },
                                    "operatorToken": {
                                        "kind": 4125,
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 25,
                                        "end": 27
                                    },
                                    "right": {
                                        "kind": 134299649,
                                        "text": "x",
                                        "rawText": "x",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 27,
                                        "end": 29
                                    },
                                    "flags": 32,
                                    "transformFlags": 128,
                                    "start": 18,
                                    "end": 29
                                },
                                "flags": 34,
                                "transformFlags": 0,
                                "start": 16,
                                "end": 30
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 16,
                            "end": 30
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 16,
                    "end": 30
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 14,
                "end": 32
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 32
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 65,
                "transformFlags": 0,
                "start": 32,
                "end": 42
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 42,
                "end": 46
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 47,
                "end": 47
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
                                "start": 50,
                                "end": 54
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
                                            "start": 54,
                                            "end": 56
                                        },
                                        "type": null,
                                        "initializer": {
                                            "kind": 220,
                                            "propertyList": {
                                                "kind": 218,
                                                "properties": [
                                                    {
                                                        "kind": 134299649,
                                                        "text": "yield",
                                                        "rawText": "yield",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 60,
                                                        "end": 65
                                                    }
                                                ],
                                                "trailingComma": false,
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 60,
                                                "end": 65
                                            },
                                            "flags": 48,
                                            "transformFlags": 8,
                                            "start": 58,
                                            "end": 66
                                        },
                                        "flags": 16,
                                        "transformFlags": 4224,
                                        "start": 54,
                                        "end": 66
                                    }
                                ],
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 54,
                                "end": 66
                            },
                            "flags": 33554448,
                            "transformFlags": 0,
                            "start": 50,
                            "end": 66
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 50,
                    "end": 66
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 48,
                "end": 68
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 32,
            "end": 68
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 65,
                "transformFlags": 0,
                "start": 68,
                "end": 78
            },
            "asteriskToken": {
                "kind": 201360950,
                "flags": 64,
                "transformFlags": 32,
                "start": 78,
                "end": 80
            },
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 80,
                "end": 83
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 84,
                "end": 84
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
                                "kind": 121,
                                "expression": {
                                    "kind": 125,
                                    "left": {
                                        "kind": 220,
                                        "propertyList": {
                                            "kind": 218,
                                            "properties": [
                                                {
                                                    "kind": 134299649,
                                                    "text": "yield",
                                                    "rawText": "yield",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 90,
                                                    "end": 95
                                                }
                                            ],
                                            "trailingComma": false,
                                            "flags": 16,
                                            "transformFlags": 0,
                                            "start": 90,
                                            "end": 95
                                        },
                                        "flags": 48,
                                        "transformFlags": 8,
                                        "start": 89,
                                        "end": 96
                                    },
                                    "operatorToken": {
                                        "kind": 4125,
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 96,
                                        "end": 98
                                    },
                                    "right": {
                                        "kind": 134299649,
                                        "text": "x",
                                        "rawText": "x",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 98,
                                        "end": 100
                                    },
                                    "flags": 32,
                                    "transformFlags": 128,
                                    "start": 89,
                                    "end": 100
                                },
                                "flags": 34,
                                "transformFlags": 0,
                                "start": 87,
                                "end": 101
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 87,
                            "end": 101
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 87,
                    "end": 101
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 85,
                "end": 103
            },
            "returnType": null,
            "flags": 272,
            "transformFlags": 0,
            "start": 68,
            "end": 103
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 65,
                "transformFlags": 0,
                "start": 103,
                "end": 113
            },
            "asteriskToken": {
                "kind": 201360950,
                "flags": 64,
                "transformFlags": 32,
                "start": 113,
                "end": 115
            },
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 115,
                "end": 118
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 119,
                "end": 119
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
                                "start": 122,
                                "end": 126
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
                                            "start": 126,
                                            "end": 128
                                        },
                                        "type": null,
                                        "initializer": {
                                            "kind": 220,
                                            "propertyList": {
                                                "kind": 218,
                                                "properties": [
                                                    {
                                                        "kind": 134299649,
                                                        "text": "yield",
                                                        "rawText": "yield",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 132,
                                                        "end": 137
                                                    }
                                                ],
                                                "trailingComma": false,
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 132,
                                                "end": 137
                                            },
                                            "flags": 48,
                                            "transformFlags": 8,
                                            "start": 130,
                                            "end": 138
                                        },
                                        "flags": 16,
                                        "transformFlags": 4224,
                                        "start": 126,
                                        "end": 138
                                    }
                                ],
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 126,
                                "end": 138
                            },
                            "flags": 33554448,
                            "transformFlags": 0,
                            "start": 122,
                            "end": 138
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 122,
                    "end": 138
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 120,
                "end": 140
            },
            "returnType": null,
            "flags": 272,
            "transformFlags": 0,
            "start": 103,
            "end": 140
        }
    ],
    "isModule": false,
    "source": "function foo() { ({yield} = x) }\n\nfunction foo() { let x = {yield} }\n\nfunction *foo() { ({yield} = x) }\n\nfunction *foo() { let x = {yield} }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 140
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Identifier expected. Reserved word in strict mode - start: 95, end: 96
✖ Identifier expected. Reserved word in strict mode - start: 137, end: 138

```

