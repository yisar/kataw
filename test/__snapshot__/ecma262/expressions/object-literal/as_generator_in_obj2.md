# Kataw parser test case

## Input

`````js

({* type(){}});

({* interface(){}});

({* in(){}});

({* of(){}});
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
                                    "start": 3,
                                    "end": 4
                                },
                                "getKeyword": null,
                                "setKeyword": null,
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "type",
                                        "rawText": "type",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 4,
                                        "end": 9
                                    },
                                    "typeParameters": null,
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [],
                                        "trailingComma": false,
                                        "flags": 160,
                                        "transformFlags": 0,
                                        "start": 10,
                                        "end": 11
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
                                            "start": 12,
                                            "end": 12
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 11,
                                        "end": 13
                                    },
                                    "flags": 160,
                                    "transformFlags": 0,
                                    "start": 9,
                                    "end": 13
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 3,
                                "end": 13
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 3,
                        "end": 13
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 2,
                    "end": 14
                },
                "flags": 35,
                "transformFlags": 0,
                "start": 0,
                "end": 15
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 16
        },
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
                                    "start": 20,
                                    "end": 21
                                },
                                "getKeyword": null,
                                "setKeyword": null,
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "interface",
                                        "rawText": "interface",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 21,
                                        "end": 31
                                    },
                                    "typeParameters": null,
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [],
                                        "trailingComma": false,
                                        "flags": 160,
                                        "transformFlags": 0,
                                        "start": 32,
                                        "end": 33
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
                                            "start": 34,
                                            "end": 34
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 33,
                                        "end": 35
                                    },
                                    "flags": 160,
                                    "transformFlags": 0,
                                    "start": 31,
                                    "end": 35
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 20,
                                "end": 35
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 20,
                        "end": 35
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 19,
                    "end": 36
                },
                "flags": 35,
                "transformFlags": 0,
                "start": 16,
                "end": 37
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 16,
            "end": 38
        },
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
                                    "start": 42,
                                    "end": 43
                                },
                                "getKeyword": null,
                                "setKeyword": null,
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "in",
                                        "rawText": "in",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 43,
                                        "end": 46
                                    },
                                    "typeParameters": null,
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [],
                                        "trailingComma": false,
                                        "flags": 160,
                                        "transformFlags": 0,
                                        "start": 47,
                                        "end": 48
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
                                            "start": 49,
                                            "end": 49
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 48,
                                        "end": 50
                                    },
                                    "flags": 160,
                                    "transformFlags": 0,
                                    "start": 46,
                                    "end": 50
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 42,
                                "end": 50
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 42,
                        "end": 50
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 41,
                    "end": 51
                },
                "flags": 35,
                "transformFlags": 0,
                "start": 38,
                "end": 52
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 38,
            "end": 53
        },
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
                                    "start": 57,
                                    "end": 58
                                },
                                "getKeyword": null,
                                "setKeyword": null,
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "of",
                                        "rawText": "of",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 58,
                                        "end": 61
                                    },
                                    "typeParameters": null,
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [],
                                        "trailingComma": false,
                                        "flags": 160,
                                        "transformFlags": 0,
                                        "start": 62,
                                        "end": 63
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
                                            "start": 64,
                                            "end": 64
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 63,
                                        "end": 65
                                    },
                                    "flags": 160,
                                    "transformFlags": 0,
                                    "start": 61,
                                    "end": 65
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 57,
                                "end": 65
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 57,
                        "end": 65
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 56,
                    "end": 66
                },
                "flags": 35,
                "transformFlags": 0,
                "start": 53,
                "end": 67
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 53,
            "end": 68
        }
    ],
    "isModule": false,
    "source": "\n({* type(){}});\n\n({* interface(){}});\n\n({* in(){}});\n\n({* of(){}});",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 68
}
```

### Printed

```javascript
({ *type() {} });
({ *interface() {} });

({ *in() {} });

({ *of() {} });

```

### Diagnostics

```javascript
✔ No errors
```

