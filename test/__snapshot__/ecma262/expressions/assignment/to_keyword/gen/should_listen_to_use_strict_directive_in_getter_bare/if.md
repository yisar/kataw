# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/gen/should_listen_to_use_strict_directive_in_getter_bare
> :: test: should listen to use strict directive in getter bare
> :: case: if
## Options

`````js
{}
`````
## Input

`````js
foo = {
  get x(){
    "use strict";
    if = x
  }
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
            "kind": 120,
            "expression": {
                "kind": 125,
                "left": {
                    "kind": 134299649,
                    "text": "foo",
                    "rawText": "foo",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 0,
                    "end": 3
                },
                "operatorToken": {
                    "kind": 4125,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 3,
                    "end": 5
                },
                "right": {
                    "kind": 220,
                    "propertyList": {
                        "kind": 218,
                        "properties": [
                            {
                                "kind": 351,
                                "asyncKeyword": null,
                                "asteriskToken": null,
                                "getKeyword": {
                                    "kind": 16498,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 7,
                                    "end": 13
                                },
                                "setKeyword": null,
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "x",
                                        "rawText": "x",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 13,
                                        "end": 15
                                    },
                                    "typeParameters": null,
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [],
                                        "trailingComma": false,
                                        "flags": 1056,
                                        "transformFlags": 0,
                                        "start": 16,
                                        "end": 17
                                    },
                                    "returnType": null,
                                    "contents": {
                                        "kind": 216,
                                        "functionStatementList": {
                                            "kind": 217,
                                            "directives": [
                                                {
                                                    "kind": 201392131,
                                                    "text": "use strict",
                                                    "rawText": "\"use strict\"",
                                                    "flags": 97,
                                                    "transformFlags": 0,
                                                    "start": 18,
                                                    "end": 35
                                                }
                                            ],
                                            "statements": [
                                                {
                                                    "kind": 164,
                                                    "ifKeyword": {
                                                        "kind": 37757019,
                                                        "flags": 81,
                                                        "transformFlags": 0,
                                                        "start": 36,
                                                        "end": 43
                                                    },
                                                    "expression": {
                                                        "kind": 125,
                                                        "left": {
                                                            "kind": 16637,
                                                            "text": "",
                                                            "rawText": "",
                                                            "flags": 64,
                                                            "transformFlags": 0,
                                                            "start": 43,
                                                            "end": 43
                                                        },
                                                        "operatorToken": {
                                                            "kind": 4125,
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 43,
                                                            "end": 45
                                                        },
                                                        "right": {
                                                            "kind": 134299649,
                                                            "text": "x",
                                                            "rawText": "x",
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 45,
                                                            "end": 47
                                                        },
                                                        "flags": 0,
                                                        "transformFlags": 128,
                                                        "start": 43,
                                                        "end": 47
                                                    },
                                                    "consequent": {
                                                        "kind": 120,
                                                        "expression": {
                                                            "kind": 16637,
                                                            "text": "",
                                                            "rawText": "",
                                                            "flags": 64,
                                                            "transformFlags": 0,
                                                            "start": 47,
                                                            "end": 47
                                                        },
                                                        "flags": 16,
                                                        "transformFlags": 4096,
                                                        "start": 47,
                                                        "end": 47
                                                    },
                                                    "elseKeyword": null,
                                                    "alternate": null,
                                                    "flags": 81,
                                                    "transformFlags": 0,
                                                    "start": 36,
                                                    "end": 47
                                                }
                                            ],
                                            "flags": 33,
                                            "transformFlags": 0,
                                            "start": 18,
                                            "end": 47
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 17,
                                        "end": 51
                                    },
                                    "flags": 1056,
                                    "transformFlags": 0,
                                    "start": 15,
                                    "end": 51
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 7,
                                "end": 51
                            }
                        ],
                        "trailingComma": false,
                        "flags": 17,
                        "transformFlags": 0,
                        "start": 7,
                        "end": 51
                    },
                    "flags": 49,
                    "transformFlags": 8,
                    "start": 5,
                    "end": 53
                },
                "flags": 0,
                "transformFlags": 128,
                "start": 0,
                "end": 53
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 53
        }
    ],
    "isModule": false,
    "source": "foo = {\n  get x(){\n    \"use strict\";\n    if = x\n  }\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 53
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Missing an opening parentheses - '( - start: 44, end: 45
✖ The left-hand side of an assignment expression must be a variable or a property access - start: 43, end: 45
✖ Declaration or statement expected - start: 50, end: 51

```

