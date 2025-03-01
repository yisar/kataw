# Kataw parser test case

## Input

`````js
type a = ({x:y} | { [x]:string}) => T;
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
            "kind": 200,
            "declareToken": null,
            "typeToken": {
                "kind": 24775,
                "flags": 64,
                "transformFlags": 0,
                "start": 0,
                "end": 4
            },
            "name": {
                "kind": 134299649,
                "text": "a",
                "rawText": "a",
                "flags": 96,
                "transformFlags": 0,
                "start": 4,
                "end": 6
            },
            "typeParameters": null,
            "assignToken": {
                "kind": 4125,
                "flags": 64,
                "transformFlags": 0,
                "start": 6,
                "end": 8
            },
            "type": {
                "kind": 139,
                "bitwiseOrToken": null,
                "bitwiseAndToken": null,
                "type": {
                    "kind": 288,
                    "typeParameters": null,
                    "arrowTypeParameterList": {
                        "kind": 292,
                        "parameters": [
                            {
                                "kind": 139,
                                "bitwiseOrToken": null,
                                "bitwiseAndToken": null,
                                "type": {
                                    "kind": 137,
                                    "types": [
                                        {
                                            "kind": 134234353,
                                            "properties": [
                                                {
                                                    "kind": 193,
                                                    "protoKeyword": null,
                                                    "staticKeyword": null,
                                                    "getKeyword": null,
                                                    "setKeyword": null,
                                                    "key": {
                                                        "kind": 134299649,
                                                        "text": "x",
                                                        "rawText": "x",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 11,
                                                        "end": 12
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
                                                                "text": "y",
                                                                "rawText": "y",
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 13,
                                                                "end": 14
                                                            },
                                                            "typeParameters": null,
                                                            "flags": 2097152,
                                                            "transformFlags": 0,
                                                            "start": 13,
                                                            "end": 14
                                                        },
                                                        "flags": 2097152,
                                                        "transformFlags": 0,
                                                        "start": 13,
                                                        "end": 14
                                                    },
                                                    "flags": 2097152,
                                                    "transformFlags": 0,
                                                    "start": 11,
                                                    "end": 14
                                                }
                                            ],
                                            "trailingComma": false,
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 10,
                                            "end": 15
                                        },
                                        {
                                            "kind": 134234353,
                                            "properties": [
                                                {
                                                    "kind": 195,
                                                    "protoKeyword": null,
                                                    "staticKeyword": null,
                                                    "key": {
                                                        "kind": 144,
                                                        "typeName": {
                                                            "kind": 134299649,
                                                            "text": "x",
                                                            "rawText": "x",
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 21,
                                                            "end": 22
                                                        },
                                                        "typeParameters": null,
                                                        "flags": 2097152,
                                                        "transformFlags": 0,
                                                        "start": 19,
                                                        "end": 22
                                                    },
                                                    "value": null,
                                                    "type": {
                                                        "kind": 139,
                                                        "bitwiseOrToken": null,
                                                        "bitwiseAndToken": null,
                                                        "type": {
                                                            "kind": 134234347,
                                                            "flags": 2097216,
                                                            "transformFlags": 0,
                                                            "start": 24,
                                                            "end": 30
                                                        },
                                                        "flags": 2097152,
                                                        "transformFlags": 0,
                                                        "start": 24,
                                                        "end": 30
                                                    },
                                                    "flags": 2097152,
                                                    "transformFlags": 0,
                                                    "start": 19,
                                                    "end": 30
                                                }
                                            ],
                                            "trailingComma": false,
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 17,
                                            "end": 31
                                        }
                                    ],
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 15,
                                    "end": 31
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 10,
                                "end": 31
                            }
                        ],
                        "trailingComma": false,
                        "flags": 2097152,
                        "transformFlags": 0,
                        "start": 8,
                        "end": 32
                    },
                    "arrowToken": {
                        "kind": 10,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 32,
                        "end": 35
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
                                "start": 35,
                                "end": 37
                            },
                            "typeParameters": null,
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 35,
                            "end": 37
                        },
                        "flags": 2097152,
                        "transformFlags": 0,
                        "start": 35,
                        "end": 37
                    },
                    "flags": 2097152,
                    "transformFlags": 0,
                    "start": 8,
                    "end": 37
                },
                "flags": 2097152,
                "transformFlags": 0,
                "start": 8,
                "end": 37
            },
            "flags": 64,
            "transformFlags": 0,
            "start": 0,
            "end": 38
        }
    ],
    "isModule": false,
    "source": "type a = ({x:y} | { [x]:string}) => T;",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 38
}
```

### Printed

```javascript
type a = ({ x: y } | { [x]: string }) => T
```

### Diagnostics

```javascript
✔ No errors
```

