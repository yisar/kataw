# Kataw parser test case

## Options

`````js
{ jsx: true, disableWebCompat: true, module: true, allowTypes: true }
`````

## Input

`````js
const f = async <T, R, S>(
  x: T,
  y: R,
  z: S,
) => {
  return null;
};
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 162,
            "lexicalKeyword": {
                "kind": 37757004,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 5
            },
            "binding": {
                "kind": 151,
                "bindingList": [
                    {
                        "kind": 190,
                        "binding": {
                            "kind": 134299649,
                            "text": "f",
                            "rawText": "f",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 5,
                            "end": 7
                        },
                        "type": null,
                        "initializer": {
                            "kind": 271,
                            "asyncKeyword": {
                                "kind": 82031,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 9,
                                "end": 15
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
                                            "start": 17,
                                            "end": 18
                                        },
                                        "type": null,
                                        "assignToken": null,
                                        "defaultType": null,
                                        "flags": 2097152,
                                        "transformFlags": 0,
                                        "start": 9,
                                        "end": 18
                                    },
                                    {
                                        "kind": 146,
                                        "name": {
                                            "kind": 134299649,
                                            "text": "R",
                                            "rawText": "R",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 19,
                                            "end": 21
                                        },
                                        "type": null,
                                        "assignToken": null,
                                        "defaultType": null,
                                        "flags": 2097152,
                                        "transformFlags": 0,
                                        "start": 19,
                                        "end": 21
                                    },
                                    {
                                        "kind": 146,
                                        "name": {
                                            "kind": 134299649,
                                            "text": "S",
                                            "rawText": "S",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 22,
                                            "end": 24
                                        },
                                        "type": null,
                                        "assignToken": null,
                                        "defaultType": null,
                                        "flags": 2097152,
                                        "transformFlags": 0,
                                        "start": 22,
                                        "end": 24
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 2097152,
                                "transformFlags": 512,
                                "start": 9,
                                "end": 25
                            },
                            "arrowPatameterList": {
                                "kind": 342,
                                "parameters": [
                                    {
                                        "kind": 281,
                                        "ellipsisToken": null,
                                        "left": {
                                            "kind": 134299649,
                                            "text": "x",
                                            "rawText": "x",
                                            "flags": 97,
                                            "transformFlags": 0,
                                            "start": 26,
                                            "end": 30
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
                                                    "start": 31,
                                                    "end": 33
                                                },
                                                "typeParameters": null,
                                                "flags": 2097152,
                                                "transformFlags": 0,
                                                "start": 31,
                                                "end": 33
                                            },
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 31,
                                            "end": 33
                                        },
                                        "right": null,
                                        "flags": 33,
                                        "transformFlags": 4096,
                                        "start": 26,
                                        "end": 33
                                    },
                                    {
                                        "kind": 281,
                                        "ellipsisToken": null,
                                        "left": {
                                            "kind": 134299649,
                                            "text": "y",
                                            "rawText": "y",
                                            "flags": 97,
                                            "transformFlags": 0,
                                            "start": 34,
                                            "end": 38
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
                                                    "text": "R",
                                                    "rawText": "R",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 39,
                                                    "end": 41
                                                },
                                                "typeParameters": null,
                                                "flags": 2097152,
                                                "transformFlags": 0,
                                                "start": 39,
                                                "end": 41
                                            },
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 39,
                                            "end": 41
                                        },
                                        "right": null,
                                        "flags": 33,
                                        "transformFlags": 4096,
                                        "start": 34,
                                        "end": 41
                                    },
                                    {
                                        "kind": 281,
                                        "ellipsisToken": null,
                                        "left": {
                                            "kind": 134299649,
                                            "text": "z",
                                            "rawText": "z",
                                            "flags": 97,
                                            "transformFlags": 0,
                                            "start": 42,
                                            "end": 46
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
                                                    "text": "S",
                                                    "rawText": "S",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 47,
                                                    "end": 49
                                                },
                                                "typeParameters": null,
                                                "flags": 2097152,
                                                "transformFlags": 0,
                                                "start": 47,
                                                "end": 49
                                            },
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 47,
                                            "end": 49
                                        },
                                        "right": null,
                                        "flags": 33,
                                        "transformFlags": 4096,
                                        "start": 42,
                                        "end": 49
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 26,
                                "end": 52
                            },
                            "returnType": null,
                            "arrowToken": {
                                "kind": 10,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 52,
                                "end": 55
                            },
                            "contents": {
                                "kind": 216,
                                "functionStatementList": {
                                    "kind": 217,
                                    "directives": [],
                                    "statements": [
                                        {
                                            "kind": 161,
                                            "returnKeyword": {
                                                "kind": 37757022,
                                                "flags": 81,
                                                "transformFlags": 0,
                                                "start": 57,
                                                "end": 66
                                            },
                                            "expression": {
                                                "kind": 138477575,
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 66,
                                                "end": 71
                                            },
                                            "flags": 81,
                                            "transformFlags": 256,
                                            "start": 57,
                                            "end": 72
                                        }
                                    ],
                                    "flags": 33,
                                    "transformFlags": 0,
                                    "start": 57,
                                    "end": 72
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 55,
                                "end": 74
                            },
                            "flags": 288,
                            "transformFlags": 0,
                            "start": 9,
                            "end": 74
                        },
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 5,
                        "end": 74
                    }
                ],
                "flags": 16777232,
                "transformFlags": 0,
                "start": 5,
                "end": 74
            },
            "flags": 33554448,
            "transformFlags": 0,
            "start": 0,
            "end": 75
        }
    ],
    "isModule": true,
    "source": "const f = async <T, R, S>(\n  x: T,\n  y: R,\n  z: S,\n) => {\n  return null;\n};",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 75
}
```

### Printed

```javascript
const f = async (x: T, y: R, z: S) => {
    return null;
  };
```

### Diagnostics

```javascript
✔ No errors
```

