# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/function/func_statements/gen/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/function/func_statements/gen/gen/in_for-in-loop
> :: test: in for-in-loop
> :: case: async function *f(){}
## Options

`````js
{}
`````
## Input

`````js
for (a in b) async function *f(){}
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 166,
            "forKeyword": {
                "kind": 37757017,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "initializer": {
                "kind": 134299649,
                "text": "a",
                "rawText": "a",
                "flags": 96,
                "transformFlags": 0,
                "start": 5,
                "end": 6
            },
            "inKeyword": {
                "kind": 21006388,
                "flags": 64,
                "transformFlags": 0,
                "start": 6,
                "end": 9
            },
            "expression": {
                "kind": 134299649,
                "text": "b",
                "rawText": "b",
                "flags": 96,
                "transformFlags": 0,
                "start": 9,
                "end": 11
            },
            "statement": {
                "kind": 176,
                "declareKeyword": null,
                "asyncKeyword": {
                    "kind": 82031,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 12,
                    "end": 18
                },
                "functionKeyword": {
                    "kind": 37822554,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 18,
                    "end": 27
                },
                "asteriskToken": {
                    "kind": 201360950,
                    "flags": 64,
                    "transformFlags": 32,
                    "start": 27,
                    "end": 29
                },
                "name": {
                    "kind": 134299649,
                    "text": "f",
                    "rawText": "f",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 29,
                    "end": 30
                },
                "typeParameters": null,
                "formalParameterList": {
                    "kind": 214,
                    "formalParameters": [],
                    "trailingComma": false,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 31,
                    "end": 31
                },
                "contents": {
                    "kind": 216,
                    "functionStatementList": {
                        "kind": 217,
                        "directives": [],
                        "statements": [],
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 33,
                        "end": 33
                    },
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 32,
                    "end": 34
                },
                "returnType": null,
                "flags": 400,
                "transformFlags": 0,
                "start": 12,
                "end": 34
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 34
        }
    ],
    "isModule": false,
    "source": "for (a in b) async function *f(){}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 34
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Function declarations cannot be used in a single-statement context - start: 12, end: 18

```

