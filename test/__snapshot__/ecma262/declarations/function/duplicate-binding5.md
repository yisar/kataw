# Kataw parser test case

## Input

`````js
function f() { { { var x } async function x() {} }}
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
                "text": "f",
                "rawText": "f",
                "flags": 96,
                "transformFlags": 0,
                "start": 8,
                "end": 10
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 11,
                "end": 11
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [
                        {
                            "kind": 124,
                            "block": {
                                "kind": 249,
                                "statements": [
                                    {
                                        "kind": 124,
                                        "block": {
                                            "kind": 249,
                                            "statements": [
                                                {
                                                    "kind": 155,
                                                    "declareKeyword": null,
                                                    "varKeyword": {
                                                        "kind": 37757002,
                                                        "flags": 80,
                                                        "transformFlags": 0,
                                                        "start": 18,
                                                        "end": 22
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
                                                                    "start": 22,
                                                                    "end": 24
                                                                },
                                                                "type": null,
                                                                "initializer": null,
                                                                "flags": 16,
                                                                "transformFlags": 4224,
                                                                "start": 22,
                                                                "end": 24
                                                            }
                                                        ],
                                                        "flags": 16,
                                                        "transformFlags": 0,
                                                        "start": 22,
                                                        "end": 24
                                                    },
                                                    "flags": 16,
                                                    "transformFlags": 0,
                                                    "start": 18,
                                                    "end": 24
                                                }
                                            ],
                                            "flags": 16,
                                            "transformFlags": 0,
                                            "start": 18,
                                            "end": 24
                                        },
                                        "flags": 16,
                                        "transformFlags": 0,
                                        "start": 16,
                                        "end": 26
                                    },
                                    {
                                        "kind": 176,
                                        "declareKeyword": null,
                                        "asyncKeyword": {
                                            "kind": 82031,
                                            "flags": 64,
                                            "transformFlags": 0,
                                            "start": 26,
                                            "end": 32
                                        },
                                        "functionKeyword": {
                                            "kind": 37822554,
                                            "flags": 64,
                                            "transformFlags": 0,
                                            "start": 32,
                                            "end": 41
                                        },
                                        "asteriskToken": null,
                                        "name": {
                                            "kind": 134299649,
                                            "text": "x",
                                            "rawText": "x",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 41,
                                            "end": 43
                                        },
                                        "typeParameters": null,
                                        "formalParameterList": {
                                            "kind": 214,
                                            "formalParameters": [],
                                            "trailingComma": false,
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 44,
                                            "end": 44
                                        },
                                        "contents": {
                                            "kind": 216,
                                            "functionStatementList": {
                                                "kind": 217,
                                                "directives": [],
                                                "statements": [],
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 47,
                                                "end": 47
                                            },
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 45,
                                            "end": 48
                                        },
                                        "returnType": null,
                                        "flags": 144,
                                        "transformFlags": 0,
                                        "start": 26,
                                        "end": 48
                                    }
                                ],
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 16,
                                "end": 48
                            },
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 14,
                            "end": 50
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 14,
                    "end": 50
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 12,
                "end": 51
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 51
        }
    ],
    "isModule": false,
    "source": "function f() { { { var x } async function x() {} }}",
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
✖ Duplicate bindingidentifier 'x' - start: 41, end: 43

```

