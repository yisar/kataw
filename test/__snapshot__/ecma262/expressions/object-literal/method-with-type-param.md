# Kataw parser test case

## Input

`````js
a={id<T>(x: T): T {}}
`````

## Options

### Parser Options

`````js
{ allowTypes : true }
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
                "kind": 125,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 0,
                    "end": 1
                },
                "operatorToken": {
                    "kind": 4125,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 1,
                    "end": 2
                },
                "right": {
                    "kind": 220,
                    "propertyList": {
                        "kind": 218,
                        "properties": [
                            {
                                "kind": 351,
                                "asyncKeyword": null,
                                "asteriskToken": null,
                                "getKeyword": null,
                                "setKeyword": null,
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "id",
                                        "rawText": "id",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 3,
                                        "end": 5
                                    },
                                    "typeParameters": {
                                        "kind": 307,
                                        "declarations": [
                                            {
                                                "kind": 146,
                                                "name": {
                                                    "kind": 134299649,
                                                    "text": "T",
                                                    "rawText": "T",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 6,
                                                    "end": 7
                                                },
                                                "type": null,
                                                "assignToken": null,
                                                "defaultType": null,
                                                "flags": 2097152,
                                                "transformFlags": 0,
                                                "start": 6,
                                                "end": 7
                                            }
                                        ],
                                        "trailingComma": false,
                                        "flags": 2097152,
                                        "transformFlags": 512,
                                        "start": 6,
                                        "end": 7
                                    },
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [
                                            {
                                                "kind": 281,
                                                "ellipsisToken": null,
                                                "left": {
                                                    "kind": 134299649,
                                                    "text": "x",
                                                    "rawText": "x",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 9,
                                                    "end": 10
                                                },
                                                "optionalToken": null,
                                                "type": {
                                                    "kind": 139,
                                                    "bitwiseOrToken": null,
                                                    "bitwiseAndToken": null,
                                                    "type": {
                                                        "kind": 144,
                                                        "typeName": {
                                                            "kind": 134299649,
                                                            "text": "T",
                                                            "rawText": "T",
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 11,
                                                            "end": 13
                                                        },
                                                        "typeParameters": null,
                                                        "flags": 2097152,
                                                        "transformFlags": 0,
                                                        "start": 11,
                                                        "end": 13
                                                    },
                                                    "flags": 2097152,
                                                    "transformFlags": 0,
                                                    "start": 11,
                                                    "end": 13
                                                },
                                                "right": null,
                                                "flags": 32,
                                                "transformFlags": 4096,
                                                "start": 9,
                                                "end": 13
                                            }
                                        ],
                                        "trailingComma": false,
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 9,
                                        "end": 14
                                    },
                                    "returnType": {
                                        "kind": 139,
                                        "bitwiseOrToken": null,
                                        "bitwiseAndToken": null,
                                        "type": {
                                            "kind": 144,
                                            "typeName": {
                                                "kind": 134299649,
                                                "text": "T",
                                                "rawText": "T",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 15,
                                                "end": 17
                                            },
                                            "typeParameters": null,
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 15,
                                            "end": 17
                                        },
                                        "flags": 2097152,
                                        "transformFlags": 0,
                                        "start": 15,
                                        "end": 17
                                    },
                                    "contents": {
                                        "kind": 216,
                                        "functionStatementList": {
                                            "kind": 217,
                                            "directives": [],
                                            "statements": [],
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 19,
                                            "end": 19
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 17,
                                        "end": 20
                                    },
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 5,
                                    "end": 20
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 3,
                                "end": 20
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 3,
                        "end": 20
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 2,
                    "end": 21
                },
                "flags": 0,
                "transformFlags": 128,
                "start": 0,
                "end": 21
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 21
        }
    ],
    "isModule": false,
    "source": "a={id<T>(x: T): T {}}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 21
}
```

### Printed

```javascript
a = { id(x: T): T {} };
```

### Diagnostics

```javascript
✔ No errors
```

