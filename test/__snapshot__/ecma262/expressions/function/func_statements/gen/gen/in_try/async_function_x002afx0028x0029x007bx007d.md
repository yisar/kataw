# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/function/func_statements/gen/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/function/func_statements/gen/gen/in_try
> :: test: in try
> :: case: async function *f(){}
## Options

`````js
{}
`````
## Input

`````js
try {
  async function *f(){}
} catch (e) {
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
            "kind": 159,
            "tryKeyword": {
                "kind": 37757027,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "block": {
                "kind": 124,
                "block": {
                    "kind": 249,
                    "statements": [
                        {
                            "kind": 176,
                            "declareKeyword": null,
                            "asyncKeyword": {
                                "kind": 82031,
                                "flags": 65,
                                "transformFlags": 0,
                                "start": 5,
                                "end": 13
                            },
                            "functionKeyword": {
                                "kind": 37822554,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 13,
                                "end": 22
                            },
                            "asteriskToken": {
                                "kind": 201360950,
                                "flags": 64,
                                "transformFlags": 32,
                                "start": 22,
                                "end": 24
                            },
                            "name": {
                                "kind": 134299649,
                                "text": "f",
                                "rawText": "f",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 24,
                                "end": 25
                            },
                            "typeParameters": null,
                            "formalParameterList": {
                                "kind": 214,
                                "formalParameters": [],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 26,
                                "end": 26
                            },
                            "contents": {
                                "kind": 216,
                                "functionStatementList": {
                                    "kind": 217,
                                    "directives": [],
                                    "statements": [],
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 28,
                                    "end": 28
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 27,
                                "end": 29
                            },
                            "returnType": null,
                            "flags": 400,
                            "transformFlags": 0,
                            "start": 5,
                            "end": 29
                        }
                    ],
                    "flags": 17,
                    "transformFlags": 0,
                    "start": 5,
                    "end": 29
                },
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 31
            },
            "catchClause": {
                "kind": 173,
                "catchKeyword": {
                    "kind": 4202575,
                    "flags": 80,
                    "transformFlags": 0,
                    "start": 31,
                    "end": 37
                },
                "catchParameter": {
                    "kind": 134299649,
                    "text": "e",
                    "rawText": "e",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 39,
                    "end": 40
                },
                "block": {
                    "kind": 124,
                    "block": {
                        "kind": 249,
                        "statements": [],
                        "flags": 17,
                        "transformFlags": 0,
                        "start": 43,
                        "end": 43
                    },
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 41,
                    "end": 45
                },
                "flags": 80,
                "transformFlags": 0,
                "start": 31,
                "end": 45
            },
            "finallyKeyword": null,
            "finallyBlock": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 45
        }
    ],
    "isModule": false,
    "source": "try {\n  async function *f(){}\n} catch (e) {\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 45
}
```

### Printed

```javascript
try {
  async function *f() {}
} catch (e) {}
```

### Diagnostics

```javascript
✔ No errors
```

