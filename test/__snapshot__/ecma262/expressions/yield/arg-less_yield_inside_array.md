# Kataw parser test case

## Input

`````js
({ *g1() {   [yield]  }})
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
                    "kind": 220,
                    "propertyList": {
                        "kind": 218,
                        "properties": [
                            {
                                "kind": 351,
                                "asyncKeyword": null,
                                "asteriskToken": {
                                    "kind": 201360950,
                                    "flags": 64,
                                    "transformFlags": 32,
                                    "start": 2,
                                    "end": 4
                                },
                                "getKeyword": null,
                                "setKeyword": null,
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "g1",
                                        "rawText": "g1",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 4,
                                        "end": 6
                                    },
                                    "typeParameters": null,
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [],
                                        "trailingComma": false,
                                        "flags": 160,
                                        "transformFlags": 0,
                                        "start": 7,
                                        "end": 8
                                    },
                                    "returnType": null,
                                    "contents": {
                                        "kind": 216,
                                        "functionStatementList": {
                                            "kind": 217,
                                            "directives": [],
                                            "statements": [
                                                {
                                                    "kind": 120,
                                                    "expression": {
                                                        "kind": 119,
                                                        "elementList": {
                                                            "kind": 270,
                                                            "elements": [
                                                                {
                                                                    "kind": 229,
                                                                    "yieldKeyword": {
                                                                        "kind": 8454253,
                                                                        "flags": 64,
                                                                        "transformFlags": 0,
                                                                        "start": 14,
                                                                        "end": 19
                                                                    },
                                                                    "delegate": false,
                                                                    "asteriskToken": null,
                                                                    "expression": null,
                                                                    "flags": 32,
                                                                    "transformFlags": 4096,
                                                                    "start": 14,
                                                                    "end": 19
                                                                }
                                                            ],
                                                            "trailingComma": false,
                                                            "flags": 32,
                                                            "transformFlags": 0,
                                                            "start": 14,
                                                            "end": 19
                                                        },
                                                        "flags": 32,
                                                        "transformFlags": 8,
                                                        "start": 10,
                                                        "end": 20
                                                    },
                                                    "flags": 16,
                                                    "transformFlags": 4096,
                                                    "start": 10,
                                                    "end": 20
                                                }
                                            ],
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 10,
                                            "end": 20
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 8,
                                        "end": 23
                                    },
                                    "flags": 160,
                                    "transformFlags": 0,
                                    "start": 6,
                                    "end": 23
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 2,
                                "end": 23
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 2,
                        "end": 23
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 1,
                    "end": 24
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 0,
                "end": 25
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 25
        }
    ],
    "isModule": false,
    "source": "({ *g1() {   [yield]  }})",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 25
}
```

### Printed

```javascript
({ *g1() {
      [yield ];
    } });
```

### Diagnostics

```javascript
✔ No errors
```

