# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/gen/inside_a_generator_func
> :: test: inside a generator func
> :: case: \u0070ackage
## Options

`````js
{}
`````
## Input

`````js
function *f(){
  \u0070ackage = x
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
                                "kind": 125,
                                "left": {
                                    "kind": 134299649,
                                    "text": "package",
                                    "rawText": "\\u0070ackage",
                                    "flags": 16481,
                                    "transformFlags": 0,
                                    "start": 14,
                                    "end": 29
                                },
                                "operatorToken": {
                                    "kind": 4125,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 29,
                                    "end": 31
                                },
                                "right": {
                                    "kind": 134299649,
                                    "text": "x",
                                    "rawText": "x",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 31,
                                    "end": 33
                                },
                                "flags": 0,
                                "transformFlags": 128,
                                "start": 14,
                                "end": 33
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 14,
                            "end": 33
                        }
                    ],
                    "flags": 16417,
                    "transformFlags": 0,
                    "start": 14,
                    "end": 33
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 13,
                "end": 35
            },
            "returnType": null,
            "flags": 272,
            "transformFlags": 0,
            "start": 0,
            "end": 35
        }
    ],
    "isModule": false,
    "source": "function *f(){\n  \\u0070ackage = x\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 35
}
```

### Printed

```javascript
function *f() {
  \u0070ackage = x;
}
```

### Diagnostics

```javascript
✔ No errors
```

