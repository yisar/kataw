# Kataw parser test case

## Input

`````js
function f(){ new.target + foo }
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
                            "kind": 120,
                            "expression": {
                                "kind": 198,
                                "left": {
                                    "kind": 211,
                                    "newKeyword": {
                                        "kind": 138477661,
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 13,
                                        "end": 17
                                    },
                                    "targetIdentifier": {
                                        "kind": 16594,
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 13,
                                        "end": 24
                                    },
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 13,
                                    "end": 24
                                },
                                "operatorToken": {
                                    "kind": 99634,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 24,
                                    "end": 26
                                },
                                "right": {
                                    "kind": 134299649,
                                    "text": "foo",
                                    "rawText": "foo",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 26,
                                    "end": 30
                                },
                                "flags": 96,
                                "transformFlags": 5120,
                                "start": 13,
                                "end": 30
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 13,
                            "end": 30
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 13,
                    "end": 30
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 12,
                "end": 32
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 32
        }
    ],
    "isModule": false,
    "source": "function f(){ new.target + foo }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 32
}
```

### Printed

```javascript
function f() {
  new.target + foo;
}
```

### Diagnostics

```javascript
✔ No errors
```

