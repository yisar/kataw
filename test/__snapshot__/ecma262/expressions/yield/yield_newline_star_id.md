# Kataw parser test case

## Input

`````js
function *f() {
  yield
  * 1;
}
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
                "text": "f",
                "rawText": "f",
                "flags": 96,
                "transformFlags": 0,
                "start": 10,
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
                                "kind": 229,
                                "yieldKeyword": {
                                    "kind": 8454253,
                                    "flags": 65,
                                    "transformFlags": 0,
                                    "start": 15,
                                    "end": 23
                                },
                                "delegate": true,
                                "asteriskToken": {
                                    "kind": 201360950,
                                    "flags": 65,
                                    "transformFlags": 32,
                                    "start": 23,
                                    "end": 27
                                },
                                "expression": {
                                    "kind": 201392130,
                                    "text": 1,
                                    "rawText": "1",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 27,
                                    "end": 29
                                },
                                "flags": 32,
                                "transformFlags": 4096,
                                "start": 15,
                                "end": 29
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 15,
                            "end": 30
                        }
                    ],
                    "flags": 33,
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
            "flags": 272,
            "transformFlags": 0,
            "start": 0,
            "end": 32
        }
    ],
    "isModule": false,
    "source": "function *f() {\n  yield\n  * 1;\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 32
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Expression expected - start: 27, end: 29

```

