# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/yield/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/yield/gen/simple
> :: test: simple
> :: case: function* gf() { switch (1) { case yield* 'foo': break; } }
## Options

`````js
{}
`````
## Input

`````js
function* gf() { switch (1) { case yield* 'foo': break; } }
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
                "end": 9
            },
            "name": {
                "kind": 134299649,
                "text": "gf",
                "rawText": "gf",
                "flags": 96,
                "transformFlags": 0,
                "start": 9,
                "end": 12
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 13,
                "end": 13
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [
                        {
                            "kind": 160,
                            "switchKeyword": {
                                "kind": 37757024,
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 16,
                                "end": 23
                            },
                            "expression": {
                                "kind": 201392130,
                                "text": 1,
                                "rawText": "1",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 25,
                                "end": 26
                            },
                            "caseBlock": {
                                "kind": 152,
                                "clauses": [
                                    {
                                        "kind": 175,
                                        "caseKeyword": {
                                            "kind": 4194382,
                                            "flags": 80,
                                            "transformFlags": 0,
                                            "start": 29,
                                            "end": 34
                                        },
                                        "expression": {
                                            "kind": 229,
                                            "yieldKeyword": {
                                                "kind": 8454253,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 34,
                                                "end": 40
                                            },
                                            "delegate": true,
                                            "asteriskToken": {
                                                "kind": 201360950,
                                                "flags": 64,
                                                "transformFlags": 32,
                                                "start": 40,
                                                "end": 41
                                            },
                                            "expression": {
                                                "kind": 201392131,
                                                "text": "foo",
                                                "rawText": "'foo'",
                                                "flags": 4194400,
                                                "transformFlags": 0,
                                                "start": 41,
                                                "end": 47
                                            },
                                            "flags": 32,
                                            "transformFlags": 4096,
                                            "start": 34,
                                            "end": 47
                                        },
                                        "colonToken": {
                                            "kind": 21,
                                            "flags": 64,
                                            "transformFlags": 0,
                                            "start": 47,
                                            "end": 48
                                        },
                                        "statements": [
                                            {
                                                "kind": 150,
                                                "breakKeyword": {
                                                    "kind": 37757005,
                                                    "flags": 80,
                                                    "transformFlags": 0,
                                                    "start": 48,
                                                    "end": 54
                                                },
                                                "label": null,
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 48,
                                                "end": 55
                                            }
                                        ],
                                        "flags": 16,
                                        "transformFlags": 0,
                                        "start": 29,
                                        "end": 55
                                    }
                                ],
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 29,
                                "end": 55
                            },
                            "flags": 80,
                            "transformFlags": 0,
                            "start": 16,
                            "end": 57
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 16,
                    "end": 57
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 14,
                "end": 59
            },
            "returnType": null,
            "flags": 272,
            "transformFlags": 0,
            "start": 0,
            "end": 59
        }
    ],
    "isModule": false,
    "source": "function* gf() { switch (1) { case yield* 'foo': break; } }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 59
}
```

### Printed

```javascript
function *gf() {
  switch (1) {
    case yield* "'foo'":
      break;
  }
}
```

### Diagnostics

```javascript
✔ No errors
```

