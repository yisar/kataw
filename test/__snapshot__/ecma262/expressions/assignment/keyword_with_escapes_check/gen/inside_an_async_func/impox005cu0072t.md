# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/gen/inside_an_async_func
> :: test: inside an async func
> :: case: impo\u0072t
## Options

`````js
{}
`````
## Input

`````js
async () => {  impo\u0072t = x  }
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
                                "kind": 263,
                                "importKeyword": {
                                    "kind": 37814364,
                                    "flags": 16464,
                                    "transformFlags": 0,
                                    "start": 13,
                                    "end": 26
                                },
                                "typeKeyword": null,
                                "typeofKeyword": null,
                                "fromClause": null,
                                "moduleSpecifier": null,
                                "importClause": null,
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 13,
                                "end": 26
                            }
                        ],
                        "flags": 16416,
                        "transformFlags": 0,
                        "start": 13,
                        "end": 26
                    },
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 11,
                    "end": 26
                },
                "flags": 288,
                "transformFlags": 0,
                "start": 0,
                "end": 26
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 26
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 28,
                "end": 30
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 28,
            "end": 30
        }
    ],
    "isModule": false,
    "source": "async () => {  impo\\u0072t = x  }",
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
✖ The `import` keyword can only be used with the module goal - start: 13, end: 28
✖ Declaration or statement expected - start: 26, end: 28
✖ '=' is not allowed here. Did you mean ';'? - start: 26, end: 28
✖ Declaration or statement expected - start: 30, end: 33

```

