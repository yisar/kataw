# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/yield/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/yield/gen/function_declaration
> :: test: function declaration
> :: case: yield 3 + yield 4;
## Options

`````js
{}
`````
## Input

`````js
function not_gen() { yield 3 + yield 4; }}
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
                "text": "not_gen",
                "rawText": "not_gen",
                "flags": 96,
                "transformFlags": 0,
                "start": 8,
                "end": 16
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 17,
                "end": 17
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
                                "kind": 134299649,
                                "text": "yield",
                                "rawText": "yield",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 20,
                                "end": 26
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 20,
                            "end": 26
                        },
                        {
                            "kind": 120,
                            "expression": {
                                "kind": 198,
                                "left": {
                                    "kind": 201392130,
                                    "text": 3,
                                    "rawText": "3",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 26,
                                    "end": 28
                                },
                                "operatorToken": {
                                    "kind": 99634,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 28,
                                    "end": 30
                                },
                                "right": {
                                    "kind": 134299649,
                                    "text": "yield",
                                    "rawText": "yield",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 30,
                                    "end": 36
                                },
                                "flags": 96,
                                "transformFlags": 5120,
                                "start": 26,
                                "end": 36
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 26,
                            "end": 36
                        },
                        {
                            "kind": 120,
                            "expression": {
                                "kind": 201392130,
                                "text": 4,
                                "rawText": "4",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 36,
                                "end": 38
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 36,
                            "end": 39
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 20,
                    "end": 39
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 18,
                "end": 41
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 41
        }
    ],
    "isModule": false,
    "source": "function not_gen() { yield 3 + yield 4; }}",
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
✖ '; ' is not allowed here. Did you mean ';'? - start: 26, end: 28
✖ '; ' is not allowed here. Did you mean ';'? - start: 36, end: 38
✖ Declaration or statement expected - start: 41, end: 42

```

