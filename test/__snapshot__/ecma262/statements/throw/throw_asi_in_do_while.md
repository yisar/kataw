# Kataw parser test case

## Input

`````js
function f() {
  do throw pass while(x);
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
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "f",
                "rawText": "f",
                "flags": 96,
                "transformFlags": 0,
                "start": 8,
                "end": 10
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 11,
                "end": 11
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [
                        {
                            "kind": 169,
                            "doKeyword": {
                                "kind": 4202580,
                                "flags": 81,
                                "transformFlags": 0,
                                "start": 14,
                                "end": 19
                            },
                            "statement": {
                                "kind": 158,
                                "throwKeyword": {
                                    "kind": 37757026,
                                    "flags": 80,
                                    "transformFlags": 0,
                                    "start": 19,
                                    "end": 25
                                },
                                "expression": {
                                    "kind": 134299649,
                                    "text": "pass",
                                    "rawText": "pass",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 25,
                                    "end": 30
                                },
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 19,
                                "end": 30
                            },
                            "whileKeyword": {
                                "kind": 37757028,
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 30,
                                "end": 36
                            },
                            "expression": {
                                "kind": 134299649,
                                "text": "x",
                                "rawText": "x",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 37,
                                "end": 38
                            },
                            "flags": 81,
                            "transformFlags": 0,
                            "start": 14,
                            "end": 40
                        }
                    ],
                    "flags": 33,
                    "transformFlags": 0,
                    "start": 14,
                    "end": 40
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 12,
                "end": 42
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 42
        }
    ],
    "isModule": false,
    "source": "function f() {\n  do throw pass while(x);\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 42
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ 'while' is not allowed here. Did you mean ';'? - start: 30, end: 36

```

