# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/gen/assign_to_paren_wrapped_keyword_in_a_generator
> :: test: assign to paren wrapped keyword in a generator
> :: case: break
## Options

`````js
{}
`````
## Input

`````js
function *f(){
  (break) = 1;
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
                                "kind": 121,
                                "expression": {
                                    "kind": 16637,
                                    "text": "",
                                    "rawText": "",
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 18,
                                    "end": 18
                                },
                                "flags": 33,
                                "transformFlags": 0,
                                "start": 14,
                                "end": 18
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 14,
                            "end": 18
                        },
                        {
                            "kind": 150,
                            "breakKeyword": {
                                "kind": 37757005,
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 18,
                                "end": 23
                            },
                            "label": {
                                "kind": 16637,
                                "text": "",
                                "rawText": "",
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 23,
                                "end": 23
                            },
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 18,
                            "end": 23
                        }
                    ],
                    "flags": 33,
                    "transformFlags": 0,
                    "start": 14,
                    "end": 23
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 13,
                "end": 23
            },
            "returnType": null,
            "flags": 272,
            "transformFlags": 0,
            "start": 0,
            "end": 23
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 1,
                "rawText": "1",
                "flags": 96,
                "transformFlags": 0,
                "start": 26,
                "end": 28
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 26,
            "end": 29
        }
    ],
    "isModule": false,
    "source": "function *f(){\n  (break) = 1;\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 31
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Identifier expected - start: 18, end: 23
✖ Identifier expected - start: 23, end: 24
✖ A 'break' statement can only jump to a label of an enclosing statement - start: 23, end: 24
✖ Declaration or statement expected - start: 24, end: 26
✖ Declaration or statement expected - start: 29, end: 31

```

