# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/gen/inside_an_async_func
> :: test: inside an async func
> :: case: sw\u0069tch
## Options

`````js
{}
`````
## Input

`````js
async () => {  sw\u0069tch = x  }
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
                "kind": 271,
                "asyncKeyword": {
                    "kind": 82031,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 0,
                    "end": 5
                },
                "typeParameters": null,
                "arrowPatameterList": {
                    "kind": 342,
                    "parameters": [],
                    "trailingComma": false,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 7,
                    "end": 7
                },
                "returnType": null,
                "arrowToken": {
                    "kind": 10,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 8,
                    "end": 11
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
                                    "flags": 16464,
                                    "transformFlags": 0,
                                    "start": 13,
                                    "end": 26
                                },
                                "expression": {
                                    "kind": 125,
                                    "left": {
                                        "kind": 16637,
                                        "text": "",
                                        "rawText": "",
                                        "flags": 64,
                                        "transformFlags": 0,
                                        "start": 26,
                                        "end": 26
                                    },
                                    "operatorToken": {
                                        "kind": 4125,
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 26,
                                        "end": 28
                                    },
                                    "right": {
                                        "kind": 134299649,
                                        "text": "x",
                                        "rawText": "x",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 28,
                                        "end": 30
                                    },
                                    "flags": 0,
                                    "transformFlags": 128,
                                    "start": 26,
                                    "end": 30
                                },
                                "caseBlock": {
                                    "kind": 152,
                                    "clauses": [],
                                    "flags": 16,
                                    "transformFlags": 0,
                                    "start": 30,
                                    "end": 30
                                },
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 13,
                                "end": 33
                            }
                        ],
                        "flags": 16416,
                        "transformFlags": 0,
                        "start": 13,
                        "end": 33
                    },
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 11,
                    "end": 33
                },
                "flags": 288,
                "transformFlags": 0,
                "start": 0,
                "end": 33
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 33
        }
    ],
    "isModule": false,
    "source": "async () => {  sw\\u0069tch = x  }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 33
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Keywords cannot contain escape characters - start: 13, end: 26
✖ Missing an opening parentheses - '( - start: 27, end: 28
✖ The left-hand side of an assignment expression must be a variable or a property access - start: 26, end: 28
✖ Declaration or statement expected - start: 32, end: 33

```

