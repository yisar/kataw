# Kataw parser test case

## Input

`````js
function* x() { function* foo(a = 1 + (yield)) {} }
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
                "end": 9
            },
            "name": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 9,
                "end": 11
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 12,
                "end": 12
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
                                "start": 15,
                                "end": 24
                            },
                            "asteriskToken": {
                                "kind": 201360950,
                                "flags": 64,
                                "transformFlags": 32,
                                "start": 24,
                                "end": 25
                            },
                            "name": {
                                "kind": 134299649,
                                "text": "foo",
                                "rawText": "foo",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 25,
                                "end": 29
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
                                            "text": "a",
                                            "rawText": "a",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 30,
                                            "end": 31
                                        },
                                        "optionalToken": null,
                                        "type": null,
                                        "right": {
                                            "kind": 198,
                                            "left": {
                                                "kind": 201392130,
                                                "text": 1,
                                                "rawText": "1",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 33,
                                                "end": 35
                                            },
                                            "operatorToken": {
                                                "kind": 99634,
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 35,
                                                "end": 37
                                            },
                                            "right": {
                                                "kind": 121,
                                                "expression": {
                                                    "kind": 229,
                                                    "yieldKeyword": {
                                                        "kind": 8454253,
                                                        "flags": 64,
                                                        "transformFlags": 0,
                                                        "start": 39,
                                                        "end": 44
                                                    },
                                                    "delegate": false,
                                                    "asteriskToken": null,
                                                    "expression": null,
                                                    "flags": 32,
                                                    "transformFlags": 4096,
                                                    "start": 39,
                                                    "end": 44
                                                },
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 37,
                                                "end": 45
                                            },
                                            "flags": 96,
                                            "transformFlags": 5120,
                                            "start": 33,
                                            "end": 45
                                        },
                                        "flags": 34,
                                        "transformFlags": 4096,
                                        "start": 30,
                                        "end": 45
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 34,
                                "transformFlags": 0,
                                "start": 30,
                                "end": 45
                            },
                            "contents": {
                                "kind": 216,
                                "functionStatementList": {
                                    "kind": 217,
                                    "directives": [],
                                    "statements": [],
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 48,
                                    "end": 48
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 46,
                                "end": 49
                            },
                            "returnType": null,
                            "flags": 272,
                            "transformFlags": 0,
                            "start": 15,
                            "end": 49
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 15,
                    "end": 49
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 13,
                "end": 51
            },
            "returnType": null,
            "flags": 272,
            "transformFlags": 0,
            "start": 0,
            "end": 51
        }
    ],
    "isModule": false,
    "source": "function* x() { function* foo(a = 1 + (yield)) {} }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 51
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ `yield` expression cannot be used in function parameters - start: 39, end: 44

```

