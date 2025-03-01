# Kataw parser test case

## Input

`````js
(async <T = U>(x) => y);
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
                "kind": 121,
                "expression": {
                    "kind": 271,
                    "asyncKeyword": {
                        "kind": 82031,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 6
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
                                    "start": 8,
                                    "end": 9
                                },
                                "type": null,
                                "assignToken": {
                                    "kind": 4125,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 9,
                                    "end": 11
                                },
                                "defaultType": {
                                    "kind": 139,
                                    "bitwiseOrToken": null,
                                    "bitwiseAndToken": null,
                                    "type": {
                                        "kind": 144,
                                        "typeName": {
                                            "kind": 134299649,
                                            "text": "U",
                                            "rawText": "U",
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
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 1,
                                "end": 13
                            }
                        ],
                        "trailingComma": false,
                        "flags": 2097152,
                        "transformFlags": 512,
                        "start": 1,
                        "end": 14
                    },
                    "arrowPatameterList": {
                        "kind": 342,
                        "parameters": [
                            {
                                "kind": 134299649,
                                "text": "x",
                                "rawText": "x",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 15,
                                "end": 16
                            }
                        ],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 15,
                        "end": 17
                    },
                    "returnType": null,
                    "arrowToken": {
                        "kind": 10,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 17,
                        "end": 20
                    },
                    "contents": {
                        "kind": 134299649,
                        "text": "y",
                        "rawText": "y",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 20,
                        "end": 22
                    },
                    "flags": 288,
                    "transformFlags": 0,
                    "start": 1,
                    "end": 22
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 0,
                "end": 23
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 24
        }
    ],
    "isModule": false,
    "source": "(async <T = U>(x) => y);",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 24
}
```

### Printed

```javascript
(async (x) => y);
```

### Diagnostics

```javascript
✔ No errors
```

