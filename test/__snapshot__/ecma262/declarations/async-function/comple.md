# Kataw parser test case

## Input

`````js
function *foo() { if (0) let
yield 0 }


async function foo() { if (0) let
await 0 }
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
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 0,
                "end": 8
            },
            "asteriskToken": {
                "kind": 201360950,
                "flags": 64,
                "transformFlags": 32,
                "start": 8,
                "end": 10
            },
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 10,
                "end": 13
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 14,
                "end": 14
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [
                        {
                            "kind": 164,
                            "ifKeyword": {
                                "kind": 37757019,
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 17,
                                "end": 20
                            },
                            "expression": {
                                "kind": 201392130,
                                "text": 0,
                                "rawText": "0",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 22,
                                "end": 23
                            },
                            "consequent": {
                                "kind": 120,
                                "expression": {
                                    "kind": 134299649,
                                    "text": "let",
                                    "rawText": "let",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 24,
                                    "end": 28
                                },
                                "flags": 16,
                                "transformFlags": 4096,
                                "start": 24,
                                "end": 28
                            },
                            "elseKeyword": null,
                            "alternate": null,
                            "flags": 80,
                            "transformFlags": 0,
                            "start": 17,
                            "end": 28
                        },
                        {
                            "kind": 120,
                            "expression": {
                                "kind": 229,
                                "yieldKeyword": {
                                    "kind": 8454253,
                                    "flags": 65,
                                    "transformFlags": 0,
                                    "start": 28,
                                    "end": 34
                                },
                                "delegate": false,
                                "asteriskToken": null,
                                "expression": {
                                    "kind": 201392130,
                                    "text": 0,
                                    "rawText": "0",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 34,
                                    "end": 36
                                },
                                "flags": 32,
                                "transformFlags": 4096,
                                "start": 28,
                                "end": 36
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 28,
                            "end": 36
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 17,
                    "end": 36
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 15,
                "end": 38
            },
            "returnType": null,
            "flags": 272,
            "transformFlags": 0,
            "start": 0,
            "end": 38
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": {
                "kind": 82031,
                "flags": 65,
                "transformFlags": 0,
                "start": 38,
                "end": 46
            },
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 46,
                "end": 55
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 55,
                "end": 59
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 60,
                "end": 60
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [
                        {
                            "kind": 164,
                            "ifKeyword": {
                                "kind": 37757019,
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 63,
                                "end": 66
                            },
                            "expression": {
                                "kind": 201392130,
                                "text": 0,
                                "rawText": "0",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 68,
                                "end": 69
                            },
                            "consequent": {
                                "kind": 120,
                                "expression": {
                                    "kind": 134299649,
                                    "text": "let",
                                    "rawText": "let",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 70,
                                    "end": 74
                                },
                                "flags": 16,
                                "transformFlags": 4096,
                                "start": 70,
                                "end": 74
                            },
                            "elseKeyword": null,
                            "alternate": null,
                            "flags": 80,
                            "transformFlags": 0,
                            "start": 63,
                            "end": 74
                        },
                        {
                            "kind": 120,
                            "expression": {
                                "kind": 208,
                                "awaitKeyword": {
                                    "kind": 82196,
                                    "flags": 65,
                                    "transformFlags": 0,
                                    "start": 74,
                                    "end": 80
                                },
                                "expression": {
                                    "kind": 201392130,
                                    "text": 0,
                                    "rawText": "0",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 80,
                                    "end": 82
                                },
                                "flags": 32,
                                "transformFlags": 4096,
                                "start": 74,
                                "end": 82
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 74,
                            "end": 82
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 63,
                    "end": 82
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 61,
                "end": 84
            },
            "returnType": null,
            "flags": 144,
            "transformFlags": 0,
            "start": 38,
            "end": 84
        }
    ],
    "isModule": false,
    "source": "function *foo() { if (0) let\nyield 0 }\n\n\nasync function foo() { if (0) let\nawait 0 }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 84
}
```

### Printed

```javascript
function *foo() {
  if (0) let;
  yield 0;
}
async function foo() {
  if (0) let;
  await 0;
}

```

### Diagnostics

```javascript
✔ No errors
```

