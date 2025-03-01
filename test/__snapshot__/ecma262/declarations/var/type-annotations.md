# Kataw parser test case

## Input

`````js
var a21: ?Array<?string>;
var identity1: <T>(x: T) => T
var identity2: <T>(x: T, ...y:T[]) => T
var a17: number[]
var a18: ?string[]
var a19: Promise<bool>[]
var x2: () => number | () => string = fn;
var x3: typeof Y = Y;
var x4: typeof Y | number = Y;
var {x5}: {x5: string; } = { x5: "hello" };
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
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "a21",
                            "rawText": "a21",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 7
                        },
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 134217970,
                                "nullableToken": {
                                    "kind": 134217750,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 8,
                                    "end": 10
                                },
                                "type": {
                                    "kind": 144,
                                    "typeName": {
                                        "kind": 134299649,
                                        "text": "Array",
                                        "rawText": "Array",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 10,
                                        "end": 15
                                    },
                                    "typeParameters": {
                                        "kind": 310,
                                        "types": [
                                            {
                                                "kind": 139,
                                                "bitwiseOrToken": null,
                                                "bitwiseAndToken": null,
                                                "type": {
                                                    "kind": 134217970,
                                                    "nullableToken": {
                                                        "kind": 134217750,
                                                        "flags": 64,
                                                        "transformFlags": 0,
                                                        "start": 16,
                                                        "end": 17
                                                    },
                                                    "type": {
                                                        "kind": 134234347,
                                                        "flags": 2097216,
                                                        "transformFlags": 0,
                                                        "start": 17,
                                                        "end": 23
                                                    },
                                                    "flags": 2097152,
                                                    "transformFlags": 0,
                                                    "start": 16,
                                                    "end": 23
                                                },
                                                "flags": 2097152,
                                                "transformFlags": 0,
                                                "start": 16,
                                                "end": 23
                                            }
                                        ],
                                        "trailingComma": false,
                                        "flags": 2097152,
                                        "transformFlags": 512,
                                        "start": 16,
                                        "end": 23
                                    },
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 10,
                                    "end": 24
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 8,
                                "end": 24
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 8,
                            "end": 24
                        },
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 3,
                        "end": 24
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 24
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 25
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 25,
                "end": 29
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "identity1",
                            "rawText": "identity1",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 29,
                            "end": 39
                        },
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 288,
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
                                                "start": 42,
                                                "end": 43
                                            },
                                            "type": null,
                                            "assignToken": null,
                                            "defaultType": null,
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 42,
                                            "end": 43
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 2097152,
                                    "transformFlags": 512,
                                    "start": 42,
                                    "end": 43
                                },
                                "arrowTypeParameterList": {
                                    "kind": 292,
                                    "parameters": [
                                        {
                                            "kind": 149,
                                            "ellipsisToken": null,
                                            "name": {
                                                "kind": 134299649,
                                                "text": "x",
                                                "rawText": "x",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 45,
                                                "end": 46
                                            },
                                            "optionalToken": null,
                                            "types": {
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
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 45,
                                            "end": 49
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 45,
                                    "end": 49
                                },
                                "arrowToken": {
                                    "kind": 10,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 50,
                                    "end": 53
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
                                            "start": 53,
                                            "end": 55
                                        },
                                        "typeParameters": null,
                                        "flags": 2097152,
                                        "transformFlags": 0,
                                        "start": 53,
                                        "end": 55
                                    },
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 53,
                                    "end": 55
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 40,
                                "end": 55
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 40,
                            "end": 55
                        },
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 29,
                        "end": 55
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 29,
                "end": 55
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 25,
            "end": 55
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 55,
                "end": 59
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "identity2",
                            "rawText": "identity2",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 59,
                            "end": 69
                        },
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 288,
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
                                                "start": 72,
                                                "end": 73
                                            },
                                            "type": null,
                                            "assignToken": null,
                                            "defaultType": null,
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 72,
                                            "end": 73
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 2097152,
                                    "transformFlags": 512,
                                    "start": 72,
                                    "end": 73
                                },
                                "arrowTypeParameterList": {
                                    "kind": 292,
                                    "parameters": [
                                        {
                                            "kind": 149,
                                            "ellipsisToken": null,
                                            "name": {
                                                "kind": 134299649,
                                                "text": "x",
                                                "rawText": "x",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 75,
                                                "end": 76
                                            },
                                            "optionalToken": null,
                                            "types": {
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
                                                        "start": 77,
                                                        "end": 79
                                                    },
                                                    "typeParameters": null,
                                                    "flags": 2097152,
                                                    "transformFlags": 0,
                                                    "start": 77,
                                                    "end": 79
                                                },
                                                "flags": 2097152,
                                                "transformFlags": 0,
                                                "start": 77,
                                                "end": 79
                                            },
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 75,
                                            "end": 79
                                        },
                                        {
                                            "kind": 149,
                                            "ellipsisToken": {
                                                "kind": 524302,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 80,
                                                "end": 84
                                            },
                                            "name": {
                                                "kind": 134299649,
                                                "text": "y",
                                                "rawText": "y",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 84,
                                                "end": 85
                                            },
                                            "optionalToken": null,
                                            "types": {
                                                "kind": 139,
                                                "bitwiseOrToken": null,
                                                "bitwiseAndToken": null,
                                                "type": {
                                                    "kind": 136,
                                                    "type": {
                                                        "kind": 144,
                                                        "typeName": {
                                                            "kind": 134299649,
                                                            "text": "T",
                                                            "rawText": "T",
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 86,
                                                            "end": 87
                                                        },
                                                        "typeParameters": null,
                                                        "flags": 2097152,
                                                        "transformFlags": 0,
                                                        "start": 86,
                                                        "end": 87
                                                    },
                                                    "flags": 2097152,
                                                    "transformFlags": 0,
                                                    "start": 86,
                                                    "end": 89
                                                },
                                                "flags": 2097152,
                                                "transformFlags": 0,
                                                "start": 86,
                                                "end": 89
                                            },
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 80,
                                            "end": 89
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 75,
                                    "end": 89
                                },
                                "arrowToken": {
                                    "kind": 10,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 90,
                                    "end": 93
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
                                            "start": 93,
                                            "end": 95
                                        },
                                        "typeParameters": null,
                                        "flags": 2097152,
                                        "transformFlags": 0,
                                        "start": 93,
                                        "end": 95
                                    },
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 93,
                                    "end": 95
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 70,
                                "end": 95
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 70,
                            "end": 95
                        },
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 59,
                        "end": 95
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 59,
                "end": 95
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 55,
            "end": 95
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 95,
                "end": 99
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "a17",
                            "rawText": "a17",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 99,
                            "end": 103
                        },
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 136,
                                "type": {
                                    "kind": 134234345,
                                    "flags": 2097216,
                                    "transformFlags": 0,
                                    "start": 104,
                                    "end": 111
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 104,
                                "end": 113
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 104,
                            "end": 113
                        },
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 99,
                        "end": 113
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 99,
                "end": 113
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 95,
            "end": 113
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 113,
                "end": 117
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "a18",
                            "rawText": "a18",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 117,
                            "end": 121
                        },
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 134217970,
                                "nullableToken": {
                                    "kind": 134217750,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 122,
                                    "end": 124
                                },
                                "type": {
                                    "kind": 136,
                                    "type": {
                                        "kind": 134234347,
                                        "flags": 2097216,
                                        "transformFlags": 0,
                                        "start": 124,
                                        "end": 130
                                    },
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 130,
                                    "end": 132
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 122,
                                "end": 132
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 122,
                            "end": 132
                        },
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 117,
                        "end": 132
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 117,
                "end": 132
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 113,
            "end": 132
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 132,
                "end": 136
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "a19",
                            "rawText": "a19",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 136,
                            "end": 140
                        },
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 136,
                                "type": {
                                    "kind": 144,
                                    "typeName": {
                                        "kind": 134299649,
                                        "text": "Promise",
                                        "rawText": "Promise",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 141,
                                        "end": 149
                                    },
                                    "typeParameters": {
                                        "kind": 310,
                                        "types": [
                                            {
                                                "kind": 139,
                                                "bitwiseOrToken": null,
                                                "bitwiseAndToken": null,
                                                "type": {
                                                    "kind": 144,
                                                    "typeName": {
                                                        "kind": 134299649,
                                                        "text": "bool",
                                                        "rawText": "bool",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 150,
                                                        "end": 154
                                                    },
                                                    "typeParameters": null,
                                                    "flags": 2097152,
                                                    "transformFlags": 0,
                                                    "start": 150,
                                                    "end": 154
                                                },
                                                "flags": 2097152,
                                                "transformFlags": 0,
                                                "start": 150,
                                                "end": 154
                                            }
                                        ],
                                        "trailingComma": false,
                                        "flags": 2097152,
                                        "transformFlags": 512,
                                        "start": 150,
                                        "end": 154
                                    },
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 141,
                                    "end": 155
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 141,
                                "end": 157
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 141,
                            "end": 157
                        },
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 136,
                        "end": 157
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 136,
                "end": 157
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 132,
            "end": 157
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 157,
                "end": 161
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "x2",
                            "rawText": "x2",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 161,
                            "end": 164
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
                                    "parameters": [],
                                    "trailingComma": false,
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 167,
                                    "end": 167
                                },
                                "arrowToken": {
                                    "kind": 10,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 168,
                                    "end": 171
                                },
                                "returnType": {
                                    "kind": 139,
                                    "bitwiseOrToken": null,
                                    "bitwiseAndToken": null,
                                    "type": {
                                        "kind": 137,
                                        "types": [
                                            {
                                                "kind": 134234345,
                                                "flags": 2097216,
                                                "transformFlags": 0,
                                                "start": 171,
                                                "end": 178
                                            },
                                            {
                                                "kind": 288,
                                                "typeParameters": null,
                                                "arrowTypeParameterList": {
                                                    "kind": 292,
                                                    "parameters": [],
                                                    "trailingComma": false,
                                                    "flags": 2097152,
                                                    "transformFlags": 0,
                                                    "start": 182,
                                                    "end": 182
                                                },
                                                "arrowToken": {
                                                    "kind": 10,
                                                    "flags": 64,
                                                    "transformFlags": 0,
                                                    "start": 183,
                                                    "end": 186
                                                },
                                                "returnType": {
                                                    "kind": 139,
                                                    "bitwiseOrToken": null,
                                                    "bitwiseAndToken": null,
                                                    "type": {
                                                        "kind": 134234347,
                                                        "flags": 2097216,
                                                        "transformFlags": 0,
                                                        "start": 186,
                                                        "end": 193
                                                    },
                                                    "flags": 2097152,
                                                    "transformFlags": 0,
                                                    "start": 186,
                                                    "end": 193
                                                },
                                                "flags": 2097152,
                                                "transformFlags": 0,
                                                "start": 180,
                                                "end": 193
                                            }
                                        ],
                                        "flags": 2097152,
                                        "transformFlags": 0,
                                        "start": 178,
                                        "end": 193
                                    },
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 171,
                                    "end": 193
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 165,
                                "end": 193
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 165,
                            "end": 193
                        },
                        "initializer": {
                            "kind": 134299649,
                            "text": "fn",
                            "rawText": "fn",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 195,
                            "end": 198
                        },
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 161,
                        "end": 198
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 161,
                "end": 198
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 157,
            "end": 199
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 199,
                "end": 203
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "x3",
                            "rawText": "x3",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 203,
                            "end": 206
                        },
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 134299891,
                                "typeOfKeyword": {
                                    "kind": 138477613,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 207,
                                    "end": 214
                                },
                                "type": {
                                    "kind": 144,
                                    "typeName": {
                                        "kind": 134299649,
                                        "text": "Y",
                                        "rawText": "Y",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 214,
                                        "end": 216
                                    },
                                    "typeParameters": null,
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 214,
                                    "end": 216
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 207,
                                "end": 216
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 207,
                            "end": 216
                        },
                        "initializer": {
                            "kind": 134299649,
                            "text": "Y",
                            "rawText": "Y",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 218,
                            "end": 220
                        },
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 203,
                        "end": 220
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 203,
                "end": 220
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 199,
            "end": 221
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 221,
                "end": 225
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "x4",
                            "rawText": "x4",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 225,
                            "end": 228
                        },
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 137,
                                "types": [
                                    {
                                        "kind": 134299891,
                                        "typeOfKeyword": {
                                            "kind": 138477613,
                                            "flags": 64,
                                            "transformFlags": 0,
                                            "start": 229,
                                            "end": 236
                                        },
                                        "type": {
                                            "kind": 144,
                                            "typeName": {
                                                "kind": 134299649,
                                                "text": "Y",
                                                "rawText": "Y",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 236,
                                                "end": 238
                                            },
                                            "typeParameters": null,
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 236,
                                            "end": 238
                                        },
                                        "flags": 2097152,
                                        "transformFlags": 0,
                                        "start": 229,
                                        "end": 238
                                    },
                                    {
                                        "kind": 134234345,
                                        "flags": 2097216,
                                        "transformFlags": 0,
                                        "start": 240,
                                        "end": 247
                                    }
                                ],
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 238,
                                "end": 247
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 229,
                            "end": 247
                        },
                        "initializer": {
                            "kind": 134299649,
                            "text": "Y",
                            "rawText": "Y",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 249,
                            "end": 251
                        },
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 225,
                        "end": 251
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 225,
                "end": 251
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 221,
            "end": 252
        },
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 81,
                "transformFlags": 0,
                "start": 252,
                "end": 256
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 212,
                            "propertyList": {
                                "kind": 213,
                                "properties": [
                                    {
                                        "kind": 134299649,
                                        "text": "x5",
                                        "rawText": "x5",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 258,
                                        "end": 260
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 258,
                                "end": 260
                            },
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 256,
                            "end": 261
                        },
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
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
                                            "text": "x5",
                                            "rawText": "x5",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 264,
                                            "end": 266
                                        },
                                        "optionalToken": null,
                                        "type": {
                                            "kind": 139,
                                            "bitwiseOrToken": null,
                                            "bitwiseAndToken": null,
                                            "type": {
                                                "kind": 134234347,
                                                "flags": 2097216,
                                                "transformFlags": 0,
                                                "start": 267,
                                                "end": 274
                                            },
                                            "flags": 2097152,
                                            "transformFlags": 0,
                                            "start": 267,
                                            "end": 274
                                        },
                                        "flags": 2097152,
                                        "transformFlags": 0,
                                        "start": 264,
                                        "end": 275
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 262,
                                "end": 277
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 262,
                            "end": 277
                        },
                        "initializer": {
                            "kind": 220,
                            "propertyList": {
                                "kind": 218,
                                "properties": [
                                    {
                                        "kind": 219,
                                        "asteriskToken": null,
                                        "left": {
                                            "kind": 134299649,
                                            "text": "x5",
                                            "rawText": "x5",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 281,
                                            "end": 284
                                        },
                                        "right": {
                                            "kind": 201392131,
                                            "text": "hello",
                                            "rawText": "\"hello\"",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 285,
                                            "end": 293
                                        },
                                        "flags": 32,
                                        "transformFlags": 128,
                                        "start": 281,
                                        "end": 293
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 281,
                                "end": 293
                            },
                            "flags": 48,
                            "transformFlags": 8,
                            "start": 279,
                            "end": 295
                        },
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 256,
                        "end": 295
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 256,
                "end": 295
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 252,
            "end": 296
        }
    ],
    "isModule": false,
    "source": "var a21: ?Array<?string>;\nvar identity1: <T>(x: T) => T\nvar identity2: <T>(x: T, ...y:T[]) => T\nvar a17: number[]\nvar a18: ?string[]\nvar a19: Promise<bool>[]\nvar x2: () => number | () => string = fn;\nvar x3: typeof Y = Y;\nvar x4: typeof Y | number = Y;\nvar {x5}: {x5: string; } = { x5: \"hello\" };",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 296
}
```

### Printed

```javascript
var a21: ? Array<? string>;
var identity1: (x: T) => T;

var identity2: (x: T, ...y: T[]) => T;

var a17: number[];

var a18: ? string[];

var a19: Promise<bool>[];

var x2: () => number | () => string = fn;

var x3: typeof Y = Y;

var x4: typeof Y | number = Y;

var { x5 }: { x5: string } = { x5: "\"hello\"" };

```

### Diagnostics

```javascript
✔ No errors
```

