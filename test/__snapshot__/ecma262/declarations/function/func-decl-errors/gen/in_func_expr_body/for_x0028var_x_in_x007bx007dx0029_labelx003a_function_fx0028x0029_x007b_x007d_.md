# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/declarations/function/func-decl-errors/autogen.md
- Path: kataw/test/__snapshot__/ecma262/declarations/function/func-decl-errors/gen/in_func_expr_body
> :: test: in func expr body
> :: case: for (var x in {}) label: function f() { };
## Options

`````js
{}
`````
## Input

`````js
(function() {for (var x in {}) label: function f() { };})()
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
                "kind": 131,
                "expression": {
                    "kind": 121,
                    "expression": {
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
                            "start": 10,
                            "end": 10
                        },
                        "contents": {
                            "kind": 216,
                            "functionStatementList": {
                                "kind": 217,
                                "directives": [],
                                "statements": [
                                    {
                                        "kind": 166,
                                        "forKeyword": {
                                            "kind": 37757017,
                                            "flags": 80,
                                            "transformFlags": 0,
                                            "start": 13,
                                            "end": 16
                                        },
                                        "initializer": {
                                            "kind": 341,
                                            "varKeyword": {
                                                "kind": 37757002,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 18,
                                                "end": 21
                                            },
                                            "declarationList": {
                                                "kind": 156,
                                                "declarations": [
                                                    {
                                                        "kind": 157,
                                                        "binding": {
                                                            "kind": 134299649,
                                                            "text": "x",
                                                            "rawText": "x",
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 21,
                                                            "end": 23
                                                        },
                                                        "type": null,
                                                        "initializer": null,
                                                        "flags": 16,
                                                        "transformFlags": 4224,
                                                        "start": 21,
                                                        "end": 23
                                                    }
                                                ],
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 21,
                                                "end": 23
                                            },
                                            "flags": 16,
                                            "transformFlags": 0,
                                            "start": 13,
                                            "end": 26
                                        },
                                        "inKeyword": {
                                            "kind": 21006388,
                                            "flags": 64,
                                            "transformFlags": 0,
                                            "start": 23,
                                            "end": 26
                                        },
                                        "expression": {
                                            "kind": 220,
                                            "propertyList": {
                                                "kind": 218,
                                                "properties": [],
                                                "trailingComma": false,
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 28,
                                                "end": 28
                                            },
                                            "flags": 48,
                                            "transformFlags": 8,
                                            "start": 26,
                                            "end": 29
                                        },
                                        "statement": {
                                            "kind": 163,
                                            "label": {
                                                "kind": 134299649,
                                                "text": "label",
                                                "rawText": "label",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 30,
                                                "end": 36
                                            },
                                            "colonToken": {
                                                "kind": 21,
                                                "flags": 64,
                                                "transformFlags": 0,
                                                "start": 36,
                                                "end": 37
                                            },
                                            "statement": {
                                                "kind": 176,
                                                "declareKeyword": null,
                                                "asyncKeyword": null,
                                                "functionKeyword": {
                                                    "kind": 37822554,
                                                    "flags": 64,
                                                    "transformFlags": 0,
                                                    "start": 37,
                                                    "end": 46
                                                },
                                                "asteriskToken": null,
                                                "name": {
                                                    "kind": 134299649,
                                                    "text": "f",
                                                    "rawText": "f",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 46,
                                                    "end": 48
                                                },
                                                "typeParameters": null,
                                                "formalParameterList": {
                                                    "kind": 214,
                                                    "formalParameters": [],
                                                    "trailingComma": false,
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 49,
                                                    "end": 49
                                                },
                                                "contents": {
                                                    "kind": 216,
                                                    "functionStatementList": {
                                                        "kind": 217,
                                                        "directives": [],
                                                        "statements": [],
                                                        "flags": 32,
                                                        "transformFlags": 0,
                                                        "start": 52,
                                                        "end": 52
                                                    },
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 50,
                                                    "end": 54
                                                },
                                                "returnType": null,
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 37,
                                                "end": 54
                                            },
                                            "flags": 16,
                                            "transformFlags": 0,
                                            "start": 30,
                                            "end": 54
                                        },
                                        "flags": 80,
                                        "transformFlags": 0,
                                        "start": 13,
                                        "end": 54
                                    },
                                    {
                                        "kind": 168,
                                        "flags": 16,
                                        "transformFlags": 0,
                                        "start": 54,
                                        "end": 55
                                    }
                                ],
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 13,
                                "end": 55
                            },
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 11,
                            "end": 56
                        },
                        "returnType": null,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 56
                    },
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 0,
                    "end": 57
                },
                "argumentList": {
                    "kind": 256,
                    "elements": [],
                    "trailingComma": false,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 58,
                    "end": 58
                },
                "flags": 32,
                "transformFlags": 1,
                "start": 0,
                "end": 59
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 59
        }
    ],
    "isModule": false,
    "source": "(function() {for (var x in {}) label: function f() { };})()",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 59
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Function declarations cannot be used in a single-statement context - start: 37, end: 46

```

