# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/gen/assigning_to_keyword_paren_wrapped
> :: test: assigning to keyword paren wrapped
> :: case: function
## Options

`````js
{}
`````
## Input

`````js
(function = x)
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
                    "kind": 125,
                    "left": {
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
                        "name": null,
                        "typeParameters": null,
                        "formalParameterList": {
                            "kind": 214,
                            "formalParameters": [],
                            "trailingComma": false,
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 9,
                            "end": 9
                        },
                        "contents": {
                            "kind": 216,
                            "functionStatementList": {
                                "kind": 217,
                                "directives": [],
                                "statements": [],
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 9,
                                "end": 9
                            },
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 9,
                            "end": 9
                        },
                        "returnType": null,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 9
                    },
                    "operatorToken": {
                        "kind": 4125,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 9,
                        "end": 11
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "x",
                        "rawText": "x",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 11,
                        "end": 13
                    },
                    "flags": 0,
                    "transformFlags": 128,
                    "start": 1,
                    "end": 13
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 0,
                "end": 14
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 14
        }
    ],
    "isModule": false,
    "source": "(function = x)",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 14
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Missing an opening parentheses - '( - start: 10, end: 11
✖ The left-hand side of an assignment expression must be a variable or a property access - start: 9, end: 11

```

