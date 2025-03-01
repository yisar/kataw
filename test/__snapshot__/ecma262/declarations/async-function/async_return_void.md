# Kataw parser test case

## Input

`````js
async function foo1(): Promise<string> {
  return;
}

async function foo2(): Promise<string> {
  return undefined;
}

async function foo3(): Promise<string> {
  function bar() { }
  return bar();
}
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
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": {
                "kind": 82031,
                "flags": 64,
                "transformFlags": 0,
                "start": 0,
                "end": 5
            },
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 5,
                "end": 14
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo1",
                "rawText": "foo1",
                "flags": 96,
                "transformFlags": 0,
                "start": 14,
                "end": 19
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 20,
                "end": 20
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
                                "start": 40,
                                "end": 49
                            },
                            "expression": null,
                            "flags": 81,
                            "transformFlags": 256,
                            "start": 40,
                            "end": 50
                        }
                    ],
                    "flags": 33,
                    "transformFlags": 0,
                    "start": 40,
                    "end": 50
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 38,
                "end": 52
            },
            "returnType": {
                "kind": 139,
                "bitwiseOrToken": null,
                "bitwiseAndToken": null,
                "type": {
                    "kind": 144,
                    "typeName": {
                        "kind": 134299649,
                        "text": "Promise",
                        "rawText": "Promise",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 22,
                        "end": 30
                    },
                    "typeParameters": {
                        "kind": 310,
                        "types": [
                            {
                                "kind": 139,
                                "bitwiseOrToken": null,
                                "bitwiseAndToken": null,
                                "type": {
                                    "kind": 134234347,
                                    "flags": 2097216,
                                    "transformFlags": 0,
                                    "start": 31,
                                    "end": 37
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 31,
                                "end": 37
                            }
                        ],
                        "trailingComma": false,
                        "flags": 2097152,
                        "transformFlags": 512,
                        "start": 31,
                        "end": 37
                    },
                    "flags": 2097152,
                    "transformFlags": 0,
                    "start": 22,
                    "end": 38
                },
                "flags": 2097152,
                "transformFlags": 0,
                "start": 22,
                "end": 38
            },
            "flags": 144,
            "transformFlags": 0,
            "start": 0,
            "end": 52
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": {
                "kind": 82031,
                "flags": 65,
                "transformFlags": 0,
                "start": 52,
                "end": 59
            },
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 59,
                "end": 68
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo2",
                "rawText": "foo2",
                "flags": 96,
                "transformFlags": 0,
                "start": 68,
                "end": 73
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 74,
                "end": 74
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
                                "start": 94,
                                "end": 103
                            },
                            "expression": {
                                "kind": 134299649,
                                "text": "undefined",
                                "rawText": "undefined",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 103,
                                "end": 113
                            },
                            "flags": 81,
                            "transformFlags": 256,
                            "start": 94,
                            "end": 114
                        }
                    ],
                    "flags": 33,
                    "transformFlags": 0,
                    "start": 94,
                    "end": 114
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 92,
                "end": 116
            },
            "returnType": {
                "kind": 139,
                "bitwiseOrToken": null,
                "bitwiseAndToken": null,
                "type": {
                    "kind": 144,
                    "typeName": {
                        "kind": 134299649,
                        "text": "Promise",
                        "rawText": "Promise",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 76,
                        "end": 84
                    },
                    "typeParameters": {
                        "kind": 310,
                        "types": [
                            {
                                "kind": 139,
                                "bitwiseOrToken": null,
                                "bitwiseAndToken": null,
                                "type": {
                                    "kind": 134234347,
                                    "flags": 2097216,
                                    "transformFlags": 0,
                                    "start": 85,
                                    "end": 91
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 85,
                                "end": 91
                            }
                        ],
                        "trailingComma": false,
                        "flags": 2097152,
                        "transformFlags": 512,
                        "start": 85,
                        "end": 91
                    },
                    "flags": 2097152,
                    "transformFlags": 0,
                    "start": 76,
                    "end": 92
                },
                "flags": 2097152,
                "transformFlags": 0,
                "start": 76,
                "end": 92
            },
            "flags": 144,
            "transformFlags": 0,
            "start": 52,
            "end": 116
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": {
                "kind": 82031,
                "flags": 65,
                "transformFlags": 0,
                "start": 116,
                "end": 123
            },
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 123,
                "end": 132
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo3",
                "rawText": "foo3",
                "flags": 96,
                "transformFlags": 0,
                "start": 132,
                "end": 137
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 138,
                "end": 138
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [
                        {
                            "kind": 176,
                            "declareKeyword": null,
                            "asyncKeyword": null,
                            "functionKeyword": {
                                "kind": 37822554,
                                "flags": 65,
                                "transformFlags": 0,
                                "start": 158,
                                "end": 169
                            },
                            "asteriskToken": null,
                            "name": {
                                "kind": 134299649,
                                "text": "bar",
                                "rawText": "bar",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 169,
                                "end": 173
                            },
                            "typeParameters": null,
                            "formalParameterList": {
                                "kind": 214,
                                "formalParameters": [],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 174,
                                "end": 174
                            },
                            "contents": {
                                "kind": 216,
                                "functionStatementList": {
                                    "kind": 217,
                                    "directives": [],
                                    "statements": [],
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 177,
                                    "end": 177
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 175,
                                "end": 179
                            },
                            "returnType": null,
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 158,
                            "end": 179
                        },
                        {
                            "kind": 161,
                            "returnKeyword": {
                                "kind": 37757022,
                                "flags": 81,
                                "transformFlags": 0,
                                "start": 179,
                                "end": 188
                            },
                            "expression": {
                                "kind": 131,
                                "expression": {
                                    "kind": 134299649,
                                    "text": "bar",
                                    "rawText": "bar",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 188,
                                    "end": 192
                                },
                                "argumentList": {
                                    "kind": 256,
                                    "elements": [],
                                    "trailingComma": false,
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 193,
                                    "end": 193
                                },
                                "flags": 32,
                                "transformFlags": 1,
                                "start": 188,
                                "end": 194
                            },
                            "flags": 81,
                            "transformFlags": 256,
                            "start": 179,
                            "end": 195
                        }
                    ],
                    "flags": 33,
                    "transformFlags": 0,
                    "start": 158,
                    "end": 195
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 156,
                "end": 197
            },
            "returnType": {
                "kind": 139,
                "bitwiseOrToken": null,
                "bitwiseAndToken": null,
                "type": {
                    "kind": 144,
                    "typeName": {
                        "kind": 134299649,
                        "text": "Promise",
                        "rawText": "Promise",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 140,
                        "end": 148
                    },
                    "typeParameters": {
                        "kind": 310,
                        "types": [
                            {
                                "kind": 139,
                                "bitwiseOrToken": null,
                                "bitwiseAndToken": null,
                                "type": {
                                    "kind": 134234347,
                                    "flags": 2097216,
                                    "transformFlags": 0,
                                    "start": 149,
                                    "end": 155
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 149,
                                "end": 155
                            }
                        ],
                        "trailingComma": false,
                        "flags": 2097152,
                        "transformFlags": 512,
                        "start": 149,
                        "end": 155
                    },
                    "flags": 2097152,
                    "transformFlags": 0,
                    "start": 140,
                    "end": 156
                },
                "flags": 2097152,
                "transformFlags": 0,
                "start": 140,
                "end": 156
            },
            "flags": 144,
            "transformFlags": 0,
            "start": 116,
            "end": 197
        }
    ],
    "isModule": false,
    "source": "async function foo1(): Promise<string> {\n  return;\n}\n\nasync function foo2(): Promise<string> {\n  return undefined;\n}\n\nasync function foo3(): Promise<string> {\n  function bar() { }\n  return bar();\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 197
}
```

### Printed

```javascript
async function foo1(): Promise<string> {
  return;
}
async function foo2(): Promise<string> {
  return undefined;
}

async function foo3(): Promise<string> {
  function bar() {}
  return bar();
}

```

### Diagnostics

```javascript
✔ No errors
```

