# Kataw parser test case

## Input

`````js
({ __proto__: null, set __proto__(x){} })
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
                                "kind": 219,
                                "asteriskToken": null,
                                "left": {
                                    "kind": 134299649,
                                    "text": "__proto__",
                                    "rawText": "__proto__",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 2,
                                    "end": 12
                                },
                                "right": {
                                    "kind": 138477575,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 13,
                                    "end": 18
                                },
                                "flags": 36,
                                "transformFlags": 128,
                                "start": 2,
                                "end": 18
                            },
                            {
                                "kind": 351,
                                "asyncKeyword": null,
                                "asteriskToken": null,
                                "getKeyword": null,
                                "setKeyword": {
                                    "kind": 16499,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 19,
                                    "end": 23
                                },
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "__proto__",
                                        "rawText": "__proto__",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 23,
                                        "end": 33
                                    },
                                    "typeParameters": null,
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [
                                            {
                                                "kind": 134299649,
                                                "text": "x",
                                                "rawText": "x",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 34,
                                                "end": 35
                                            }
                                        ],
                                        "trailingComma": false,
                                        "flags": 608,
                                        "transformFlags": 0,
                                        "start": 34,
                                        "end": 36
                                    },
                                    "returnType": null,
                                    "contents": {
                                        "kind": 216,
                                        "functionStatementList": {
                                            "kind": 217,
                                            "directives": [],
                                            "statements": [],
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 37,
                                            "end": 37
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 36,
                                        "end": 38
                                    },
                                    "flags": 544,
                                    "transformFlags": 0,
                                    "start": 33,
                                    "end": 38
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 19,
                                "end": 38
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 2,
                        "end": 38
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 1,
                    "end": 40
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 0,
                "end": 41
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 41
        }
    ],
    "isModule": false,
    "source": "({ __proto__: null, set __proto__(x){} })",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 41
}
```

### Printed

```javascript
({ __proto__: null, set __proto__(x) {} });
```

### Diagnostics

```javascript
✔ No errors
```

