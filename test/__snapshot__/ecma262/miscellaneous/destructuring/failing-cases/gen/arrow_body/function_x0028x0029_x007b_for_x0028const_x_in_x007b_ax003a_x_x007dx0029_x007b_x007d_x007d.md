# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/miscellaneous/destructuring/failing-cases/autogen.md
- Path: kataw/test/__snapshot__/ecma262/miscellaneous/destructuring/failing-cases/gen/arrow_body
> :: test: arrow body
> :: case: function () { for (const x in { a: x }) { } }
## Options

`````js
{}
`````
## Input

`````js
(x, function () { for (const x in { a: x }) { } }) => function () { for (const x in { a: x }) { } }
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 132,
                    "expressions": [
                        {
                            "kind": 134299649,
                            "text": "x",
                            "rawText": "x",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 1,
                            "end": 2
                        },
                        {
                            "kind": 177,
                            "asyncKeyword": null,
                            "functionKeyword": {
                                "kind": 37822554,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 3,
                                "end": 12
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
                                "start": 14,
                                "end": 14
                            },
                            "contents": {
                                "kind": 216,
                                "functionStatementList": {
                                    "kind": 217,
                                    "directives": [],
                                    "statements": [
                                        {
                                            "kind": 166,
                                            "forKeyword": {
                                                "kind": 37757017,
                                                "flags": 80,
                                                "transformFlags": 0,
                                                "start": 17,
                                                "end": 21
                                            },
                                            "initializer": {
                                                "kind": 162,
                                                "lexicalKeyword": {
                                                    "kind": 37757004,
                                                    "flags": 64,
                                                    "transformFlags": 0,
                                                    "start": 23,
                                                    "end": 28
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
                                                                "start": 28,
                                                                "end": 30
                                                            },
                                                            "type": null,
                                                            "initializer": null,
                                                            "flags": 16,
                                                            "transformFlags": 4224,
                                                            "start": 28,
                                                            "end": 30
                                                        }
                                                    ],
                                                    "flags": 16777232,
                                                    "transformFlags": 0,
                                                    "start": 28,
                                                    "end": 30
                                                },
                                                "flags": 33554448,
                                                "transformFlags": 0,
                                                "start": 17,
                                                "end": 30
                                            },
                                            "inKeyword": {
                                                "kind": 21006388,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 30,
                                                "end": 33
                                            },
                                            "expression": {
                                                "kind": 220,
                                                "propertyList": {
                                                    "kind": 218,
                                                    "properties": [
                                                        {
                                                            "kind": 219,
                                                            "asteriskToken": null,
                                                            "left": {
                                                                "kind": 134299649,
                                                                "text": "a",
                                                                "rawText": "a",
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 35,
                                                                "end": 37
                                                            },
                                                            "right": {
                                                                "kind": 134299649,
                                                                "text": "x",
                                                                "rawText": "x",
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 38,
                                                                "end": 40
                                                            },
                                                            "flags": 32,
                                                            "transformFlags": 128,
                                                            "start": 35,
                                                            "end": 40
                                                        }
                                                    ],
                                                    "trailingComma": false,
                                                    "flags": 16,
                                                    "transformFlags": 0,
                                                    "start": 35,
                                                    "end": 40
                                                },
                                                "flags": 48,
                                                "transformFlags": 8,
                                                "start": 33,
                                                "end": 42
                                            },
                                            "statement": {
                                                "kind": 124,
                                                "block": {
                                                    "kind": 249,
                                                    "statements": [],
                                                    "flags": 16,
                                                    "transformFlags": 0,
                                                    "start": 45,
                                                    "end": 45
                                                },
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 43,
                                                "end": 47
                                            },
                                            "flags": 80,
                                            "transformFlags": 0,
                                            "start": 17,
                                            "end": 47
                                        }
                                    ],
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 17,
                                    "end": 47
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 15,
                                "end": 49
                            },
                            "returnType": null,
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 49
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 1024,
                    "start": 0,
                    "end": 49
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 0,
                "end": 50
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 50
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 53,
                "end": 62
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
                "start": 64,
                "end": 64
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [
                        {
                            "kind": 166,
                            "forKeyword": {
                                "kind": 37757017,
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 67,
                                "end": 71
                            },
                            "initializer": {
                                "kind": 162,
                                "lexicalKeyword": {
                                    "kind": 37757004,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 73,
                                    "end": 78
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
                                                "start": 78,
                                                "end": 80
                                            },
                                            "type": null,
                                            "initializer": null,
                                            "flags": 16,
                                            "transformFlags": 4224,
                                            "start": 78,
                                            "end": 80
                                        }
                                    ],
                                    "flags": 16777232,
                                    "transformFlags": 0,
                                    "start": 78,
                                    "end": 80
                                },
                                "flags": 33554448,
                                "transformFlags": 0,
                                "start": 67,
                                "end": 80
                            },
                            "inKeyword": {
                                "kind": 21006388,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 80,
                                "end": 83
                            },
                            "expression": {
                                "kind": 220,
                                "propertyList": {
                                    "kind": 218,
                                    "properties": [
                                        {
                                            "kind": 219,
                                            "asteriskToken": null,
                                            "left": {
                                                "kind": 134299649,
                                                "text": "a",
                                                "rawText": "a",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 85,
                                                "end": 87
                                            },
                                            "right": {
                                                "kind": 134299649,
                                                "text": "x",
                                                "rawText": "x",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 88,
                                                "end": 90
                                            },
                                            "flags": 32,
                                            "transformFlags": 128,
                                            "start": 85,
                                            "end": 90
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 16,
                                    "transformFlags": 0,
                                    "start": 85,
                                    "end": 90
                                },
                                "flags": 48,
                                "transformFlags": 8,
                                "start": 83,
                                "end": 92
                            },
                            "statement": {
                                "kind": 124,
                                "block": {
                                    "kind": 249,
                                    "statements": [],
                                    "flags": 16,
                                    "transformFlags": 0,
                                    "start": 95,
                                    "end": 95
                                },
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 93,
                                "end": 97
                            },
                            "flags": 80,
                            "transformFlags": 0,
                            "start": 67,
                            "end": 97
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 67,
                    "end": 97
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 65,
                "end": 99
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 53,
            "end": 99
        }
    ],
    "isModule": false,
    "source": "(x, function () { for (const x in { a: x }) { } }) => function () { for (const x in { a: x }) { } }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 99
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ '=>' is not allowed here. Did you mean ';'? - start: 50, end: 53
✖ Binding identifier expected - start: 62, end: 64

```

