# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/miscellaneous/should-fail/autogen.md
- Path: kataw/test/__snapshot__/ecma262/miscellaneous/should-fail/gen/in_a_block
> :: test: in a block
> :: case: if (true) function* g() {  } else ;
## Options

`````js
{}
`````
## Input

`````js
{ if (true) function* g() {  } else ; }
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 124,
            "block": {
                "kind": 249,
                "statements": [
                    {
                        "kind": 164,
                        "ifKeyword": {
                            "kind": 37757019,
                            "flags": 80,
                            "transformFlags": 0,
                            "start": 1,
                            "end": 4
                        },
                        "expression": {
                            "kind": 24752947,
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 6,
                            "end": 10
                        },
                        "consequent": {
                            "kind": 176,
                            "declareKeyword": null,
                            "asyncKeyword": null,
                            "functionKeyword": {
                                "kind": 37822554,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 11,
                                "end": 20
                            },
                            "asteriskToken": {
                                "kind": 201360950,
                                "flags": 64,
                                "transformFlags": 32,
                                "start": 20,
                                "end": 21
                            },
                            "name": {
                                "kind": 134299649,
                                "text": "g",
                                "rawText": "g",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 21,
                                "end": 23
                            },
                            "typeParameters": null,
                            "formalParameterList": {
                                "kind": 214,
                                "formalParameters": [],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 24,
                                "end": 24
                            },
                            "contents": {
                                "kind": 216,
                                "functionStatementList": {
                                    "kind": 217,
                                    "directives": [],
                                    "statements": [],
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 27,
                                    "end": 27
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 25,
                                "end": 30
                            },
                            "returnType": null,
                            "flags": 272,
                            "transformFlags": 0,
                            "start": 11,
                            "end": 30
                        },
                        "elseKeyword": {
                            "kind": 4194389,
                            "flags": 64,
                            "transformFlags": 0,
                            "start": 30,
                            "end": 35
                        },
                        "alternate": {
                            "kind": 168,
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 35,
                            "end": 37
                        },
                        "flags": 80,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 37
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 1,
                "end": 37
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 39
        }
    ],
    "isModule": false,
    "source": "{ if (true) function* g() {  } else ; }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 39
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Generators can only be declared at the top level or inside a block - start: 21, end: 23

```

