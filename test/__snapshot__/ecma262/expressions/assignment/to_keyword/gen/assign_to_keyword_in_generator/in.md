# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/gen/assign_to_keyword_in_generator
> :: test: assign to keyword in generator
> :: case: in
## Options

`````js
{}
`````
## Input

`````js
function *f(){
  in = 1;
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
                                "kind": 198,
                                "left": {
                                    "kind": 16637,
                                    "text": "",
                                    "rawText": "",
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 14,
                                    "end": 14
                                },
                                "operatorToken": {
                                    "kind": 21006388,
                                    "flags": 97,
                                    "transformFlags": 0,
                                    "start": 14,
                                    "end": 19
                                },
                                "right": {
                                    "kind": 16637,
                                    "text": "",
                                    "rawText": "",
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 19,
                                    "end": 19
                                },
                                "flags": 97,
                                "transformFlags": 5120,
                                "start": 14,
                                "end": 19
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 14,
                            "end": 19
                        }
                    ],
                    "flags": 33,
                    "transformFlags": 0,
                    "start": 14,
                    "end": 19
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 13,
                "end": 19
            },
            "returnType": null,
            "flags": 272,
            "transformFlags": 0,
            "start": 0,
            "end": 19
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 1,
                "rawText": "1",
                "flags": 96,
                "transformFlags": 0,
                "start": 21,
                "end": 23
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 21,
            "end": 24
        }
    ],
    "isModule": false,
    "source": "function *f(){\n  in = 1;\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 26
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Identifier expected - start: 14, end: 19
✖ Identifier expected - start: 19, end: 21
✖ Declaration or statement expected - start: 24, end: 26

```

