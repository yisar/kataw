# Kataw parser test case

## Input

`````js
(function f() { (yield => {}); });
(function f() { ((yield, ...a) => {}); });
(function f() { (([yield]) => {}); });
(function f() { (({yield}) => {}); });
(function f() { ((yield) => {}); });
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
                    "kind": 177,
                    "asyncKeyword": null,
                    "functionKeyword": {
                        "kind": 37822554,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 9
                    },
                    "asteriskToken": null,
                    "name": {
                        "kind": 134299649,
                        "text": "f",
                        "rawText": "f",
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
                                    "kind": 120,
                                    "expression": {
                                        "kind": 121,
                                        "expression": {
                                            "kind": 271,
                                            "asyncKeyword": null,
                                            "typeParameters": null,
                                            "arrowPatameterList": {
                                                "kind": 134299649,
                                                "text": "yield",
                                                "rawText": "yield",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 17,
                                                "end": 22
                                            },
                                            "returnType": null,
                                            "arrowToken": {
                                                "kind": 10,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 22,
                                                "end": 25
                                            },
                                            "contents": {
                                                "kind": 216,
                                                "functionStatementList": {
                                                    "kind": 217,
                                                    "directives": [],
                                                    "statements": [],
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 27,
                                                    "end": 27
                                                },
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 25,
                                                "end": 28
                                            },
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 17,
                                            "end": 28
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 15,
                                        "end": 29
                                    },
                                    "flags": 16,
                                    "transformFlags": 4096,
                                    "start": 15,
                                    "end": 30
                                }
                            ],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 15,
                            "end": 30
                        },
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 13,
                        "end": 32
                    },
                    "returnType": null,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 1,
                    "end": 32
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 0,
                "end": 33
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 34
        },
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 177,
                    "asyncKeyword": null,
                    "functionKeyword": {
                        "kind": 37822554,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 36,
                        "end": 44
                    },
                    "asteriskToken": null,
                    "name": {
                        "kind": 134299649,
                        "text": "f",
                        "rawText": "f",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 44,
                        "end": 46
                    },
                    "typeParameters": null,
                    "formalParameterList": {
                        "kind": 214,
                        "formalParameters": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 47,
                        "end": 47
                    },
                    "contents": {
                        "kind": 216,
                        "functionStatementList": {
                            "kind": 217,
                            "directives": [],
                            "statements": [
                                {
                                    "kind": 120,
                                    "expression": {
                                        "kind": 121,
                                        "expression": {
                                            "kind": 271,
                                            "asyncKeyword": null,
                                            "typeParameters": null,
                                            "arrowPatameterList": {
                                                "kind": 342,
                                                "parameters": [
                                                    {
                                                        "kind": 134299649,
                                                        "text": "yield",
                                                        "rawText": "yield",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 53,
                                                        "end": 58
                                                    },
                                                    {
                                                        "kind": 281,
                                                        "ellipsisToken": {
                                                            "kind": 524302,
                                                            "flags": 64,
                                                            "transformFlags": 0,
                                                            "start": 59,
                                                            "end": 63
                                                        },
                                                        "left": {
                                                            "kind": 134299649,
                                                            "text": "a",
                                                            "rawText": "a",
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 63,
                                                            "end": 64
                                                        },
                                                        "optionalToken": null,
                                                        "type": null,
                                                        "right": null,
                                                        "flags": 34,
                                                        "transformFlags": 4096,
                                                        "start": 59,
                                                        "end": 64
                                                    }
                                                ],
                                                "trailingComma": false,
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 53,
                                                "end": 65
                                            },
                                            "returnType": null,
                                            "arrowToken": {
                                                "kind": 10,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 65,
                                                "end": 68
                                            },
                                            "contents": {
                                                "kind": 216,
                                                "functionStatementList": {
                                                    "kind": 217,
                                                    "directives": [],
                                                    "statements": [],
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 70,
                                                    "end": 70
                                                },
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 68,
                                                "end": 71
                                            },
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 52,
                                            "end": 71
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 50,
                                        "end": 72
                                    },
                                    "flags": 16,
                                    "transformFlags": 4096,
                                    "start": 50,
                                    "end": 73
                                }
                            ],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 50,
                            "end": 73
                        },
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 48,
                        "end": 75
                    },
                    "returnType": null,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 36,
                    "end": 75
                },
                "flags": 33,
                "transformFlags": 0,
                "start": 34,
                "end": 76
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 34,
            "end": 77
        },
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 177,
                    "asyncKeyword": null,
                    "functionKeyword": {
                        "kind": 37822554,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 79,
                        "end": 87
                    },
                    "asteriskToken": null,
                    "name": {
                        "kind": 134299649,
                        "text": "f",
                        "rawText": "f",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 87,
                        "end": 89
                    },
                    "typeParameters": null,
                    "formalParameterList": {
                        "kind": 214,
                        "formalParameters": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 90,
                        "end": 90
                    },
                    "contents": {
                        "kind": 216,
                        "functionStatementList": {
                            "kind": 217,
                            "directives": [],
                            "statements": [
                                {
                                    "kind": 120,
                                    "expression": {
                                        "kind": 121,
                                        "expression": {
                                            "kind": 271,
                                            "asyncKeyword": null,
                                            "typeParameters": null,
                                            "arrowPatameterList": {
                                                "kind": 342,
                                                "parameters": [
                                                    {
                                                        "kind": 201,
                                                        "elementList": {
                                                            "kind": 270,
                                                            "elements": [
                                                                {
                                                                    "kind": 134299649,
                                                                    "text": "yield",
                                                                    "rawText": "yield",
                                                                    "flags": 96,
                                                                    "transformFlags": 0,
                                                                    "start": 97,
                                                                    "end": 102
                                                                }
                                                            ],
                                                            "trailingComma": false,
                                                            "flags": 32,
                                                            "transformFlags": 0,
                                                            "start": 97,
                                                            "end": 102
                                                        },
                                                        "flags": 32,
                                                        "transformFlags": 0,
                                                        "start": 96,
                                                        "end": 103
                                                    }
                                                ],
                                                "trailingComma": false,
                                                "flags": 34,
                                                "transformFlags": 0,
                                                "start": 96,
                                                "end": 104
                                            },
                                            "returnType": null,
                                            "arrowToken": {
                                                "kind": 10,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 104,
                                                "end": 107
                                            },
                                            "contents": {
                                                "kind": 216,
                                                "functionStatementList": {
                                                    "kind": 217,
                                                    "directives": [],
                                                    "statements": [],
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 109,
                                                    "end": 109
                                                },
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 107,
                                                "end": 110
                                            },
                                            "flags": 34,
                                            "transformFlags": 0,
                                            "start": 95,
                                            "end": 110
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 93,
                                        "end": 111
                                    },
                                    "flags": 16,
                                    "transformFlags": 4096,
                                    "start": 93,
                                    "end": 112
                                }
                            ],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 93,
                            "end": 112
                        },
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 91,
                        "end": 114
                    },
                    "returnType": null,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 79,
                    "end": 114
                },
                "flags": 33,
                "transformFlags": 0,
                "start": 77,
                "end": 115
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 77,
            "end": 116
        },
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 177,
                    "asyncKeyword": null,
                    "functionKeyword": {
                        "kind": 37822554,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 118,
                        "end": 126
                    },
                    "asteriskToken": null,
                    "name": {
                        "kind": 134299649,
                        "text": "f",
                        "rawText": "f",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 126,
                        "end": 128
                    },
                    "typeParameters": null,
                    "formalParameterList": {
                        "kind": 214,
                        "formalParameters": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 129,
                        "end": 129
                    },
                    "contents": {
                        "kind": 216,
                        "functionStatementList": {
                            "kind": 217,
                            "directives": [],
                            "statements": [
                                {
                                    "kind": 120,
                                    "expression": {
                                        "kind": 121,
                                        "expression": {
                                            "kind": 271,
                                            "asyncKeyword": null,
                                            "typeParameters": null,
                                            "arrowPatameterList": {
                                                "kind": 342,
                                                "parameters": [
                                                    {
                                                        "kind": 212,
                                                        "propertyList": {
                                                            "kind": 213,
                                                            "properties": [
                                                                {
                                                                    "kind": 134299649,
                                                                    "text": "yield",
                                                                    "rawText": "yield",
                                                                    "flags": 96,
                                                                    "transformFlags": 0,
                                                                    "start": 136,
                                                                    "end": 141
                                                                }
                                                            ],
                                                            "trailingComma": false,
                                                            "flags": 32,
                                                            "transformFlags": 0,
                                                            "start": 136,
                                                            "end": 141
                                                        },
                                                        "flags": 48,
                                                        "transformFlags": 0,
                                                        "start": 135,
                                                        "end": 142
                                                    }
                                                ],
                                                "trailingComma": false,
                                                "flags": 34,
                                                "transformFlags": 0,
                                                "start": 135,
                                                "end": 143
                                            },
                                            "returnType": null,
                                            "arrowToken": {
                                                "kind": 10,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 143,
                                                "end": 146
                                            },
                                            "contents": {
                                                "kind": 216,
                                                "functionStatementList": {
                                                    "kind": 217,
                                                    "directives": [],
                                                    "statements": [],
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 148,
                                                    "end": 148
                                                },
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 146,
                                                "end": 149
                                            },
                                            "flags": 34,
                                            "transformFlags": 0,
                                            "start": 134,
                                            "end": 149
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 132,
                                        "end": 150
                                    },
                                    "flags": 16,
                                    "transformFlags": 4096,
                                    "start": 132,
                                    "end": 151
                                }
                            ],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 132,
                            "end": 151
                        },
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 130,
                        "end": 153
                    },
                    "returnType": null,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 118,
                    "end": 153
                },
                "flags": 33,
                "transformFlags": 0,
                "start": 116,
                "end": 154
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 116,
            "end": 155
        },
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 177,
                    "asyncKeyword": null,
                    "functionKeyword": {
                        "kind": 37822554,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 157,
                        "end": 165
                    },
                    "asteriskToken": null,
                    "name": {
                        "kind": 134299649,
                        "text": "f",
                        "rawText": "f",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 165,
                        "end": 167
                    },
                    "typeParameters": null,
                    "formalParameterList": {
                        "kind": 214,
                        "formalParameters": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 168,
                        "end": 168
                    },
                    "contents": {
                        "kind": 216,
                        "functionStatementList": {
                            "kind": 217,
                            "directives": [],
                            "statements": [
                                {
                                    "kind": 120,
                                    "expression": {
                                        "kind": 121,
                                        "expression": {
                                            "kind": 271,
                                            "asyncKeyword": null,
                                            "typeParameters": null,
                                            "arrowPatameterList": {
                                                "kind": 342,
                                                "parameters": [
                                                    {
                                                        "kind": 134299649,
                                                        "text": "yield",
                                                        "rawText": "yield",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 174,
                                                        "end": 179
                                                    }
                                                ],
                                                "trailingComma": false,
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 174,
                                                "end": 180
                                            },
                                            "returnType": null,
                                            "arrowToken": {
                                                "kind": 10,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 180,
                                                "end": 183
                                            },
                                            "contents": {
                                                "kind": 216,
                                                "functionStatementList": {
                                                    "kind": 217,
                                                    "directives": [],
                                                    "statements": [],
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 185,
                                                    "end": 185
                                                },
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 183,
                                                "end": 186
                                            },
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 173,
                                            "end": 186
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 171,
                                        "end": 187
                                    },
                                    "flags": 16,
                                    "transformFlags": 4096,
                                    "start": 171,
                                    "end": 188
                                }
                            ],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 171,
                            "end": 188
                        },
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 169,
                        "end": 190
                    },
                    "returnType": null,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 157,
                    "end": 190
                },
                "flags": 33,
                "transformFlags": 0,
                "start": 155,
                "end": 191
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 155,
            "end": 192
        }
    ],
    "isModule": false,
    "source": "(function f() { (yield => {}); });\n(function f() { ((yield, ...a) => {}); });\n(function f() { (([yield]) => {}); });\n(function f() { (({yield}) => {}); });\n(function f() { ((yield) => {}); });",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 192
}
```

### Printed

```javascript
(function f() {
    (yield => {});
  });
(function f() {
    ((yield, ...a) => {});
  });

(function f() {
    (([yield]) => {});
  });

(function f() {
    (({ yield }) => {});
  });

(function f() {
    ((yield) => {});
  });

```

### Diagnostics

```javascript
✔ No errors
```

