# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/super/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/super/gen/obj-expr-set
> :: test: obj-expr-set
> :: case: class C { set x(_) { super(
## Options

`````js
{}
`````
## Input

`````js
({ set x(_) { class C { set x(_) { super( } })
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
                    "kind": 220,
                    "propertyList": {
                        "kind": 218,
                        "properties": [
                            {
                                "kind": 351,
                                "asyncKeyword": null,
                                "asteriskToken": null,
                                "getKeyword": null,
                                "setKeyword": {
                                    "kind": 16499,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 2,
                                    "end": 6
                                },
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "x",
                                        "rawText": "x",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 6,
                                        "end": 8
                                    },
                                    "typeParameters": null,
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [
                                            {
                                                "kind": 134299649,
                                                "text": "_",
                                                "rawText": "_",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 9,
                                                "end": 10
                                            }
                                        ],
                                        "trailingComma": false,
                                        "flags": 608,
                                        "transformFlags": 0,
                                        "start": 9,
                                        "end": 11
                                    },
                                    "returnType": null,
                                    "contents": {
                                        "kind": 216,
                                        "functionStatementList": {
                                            "kind": 217,
                                            "directives": [],
                                            "statements": [
                                                {
                                                    "kind": 178,
                                                    "declareKeyword": null,
                                                    "decorators": null,
                                                    "classKeyword": {
                                                        "kind": 37822544,
                                                        "flags": 80,
                                                        "transformFlags": 0,
                                                        "start": 13,
                                                        "end": 19
                                                    },
                                                    "name": {
                                                        "kind": 134299649,
                                                        "text": "C",
                                                        "rawText": "C",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 19,
                                                        "end": 21
                                                    },
                                                    "typeParameters": null,
                                                    "tail": {
                                                        "kind": 277,
                                                        "classHeritage": null,
                                                        "body": {
                                                            "kind": 303,
                                                            "elements": [
                                                                {
                                                                    "kind": 278,
                                                                    "declareToken": null,
                                                                    "decorators": null,
                                                                    "staticKeyword": null,
                                                                    "asyncKeyword": null,
                                                                    "setKeyword": null,
                                                                    "getKeyword": {
                                                                        "kind": 16499,
                                                                        "flags": 64,
                                                                        "transformFlags": 0,
                                                                        "start": 23,
                                                                        "end": 27
                                                                    },
                                                                    "asteriskToken": null,
                                                                    "method": {
                                                                        "kind": 209,
                                                                        "name": {
                                                                            "kind": 134299649,
                                                                            "text": "x",
                                                                            "rawText": "x",
                                                                            "flags": 96,
                                                                            "transformFlags": 0,
                                                                            "start": 27,
                                                                            "end": 29
                                                                        },
                                                                        "typeParameters": null,
                                                                        "formalParameterList": {
                                                                            "kind": 214,
                                                                            "formalParameters": [
                                                                                {
                                                                                    "kind": 134299649,
                                                                                    "text": "_",
                                                                                    "rawText": "_",
                                                                                    "flags": 96,
                                                                                    "transformFlags": 0,
                                                                                    "start": 30,
                                                                                    "end": 31
                                                                                }
                                                                            ],
                                                                            "trailingComma": false,
                                                                            "flags": 608,
                                                                            "transformFlags": 0,
                                                                            "start": 30,
                                                                            "end": 32
                                                                        },
                                                                        "returnType": null,
                                                                        "contents": {
                                                                            "kind": 216,
                                                                            "functionStatementList": {
                                                                                "kind": 217,
                                                                                "directives": [],
                                                                                "statements": [
                                                                                    {
                                                                                        "kind": 120,
                                                                                        "expression": {
                                                                                            "kind": 131,
                                                                                            "expression": {
                                                                                                "kind": 4259935,
                                                                                                "flags": 96,
                                                                                                "transformFlags": 0,
                                                                                                "start": 34,
                                                                                                "end": 40
                                                                                            },
                                                                                            "argumentList": {
                                                                                                "kind": 256,
                                                                                                "elements": [],
                                                                                                "trailingComma": false,
                                                                                                "flags": 32,
                                                                                                "transformFlags": 0,
                                                                                                "start": 41,
                                                                                                "end": 41
                                                                                            },
                                                                                            "flags": 32,
                                                                                            "transformFlags": 1,
                                                                                            "start": 34,
                                                                                            "end": 41
                                                                                        },
                                                                                        "flags": 16,
                                                                                        "transformFlags": 4096,
                                                                                        "start": 34,
                                                                                        "end": 41
                                                                                    }
                                                                                ],
                                                                                "flags": 32,
                                                                                "transformFlags": 0,
                                                                                "start": 34,
                                                                                "end": 41
                                                                            },
                                                                            "flags": 32,
                                                                            "transformFlags": 0,
                                                                            "start": 32,
                                                                            "end": 43
                                                                        },
                                                                        "flags": 512,
                                                                        "transformFlags": 0,
                                                                        "start": 29,
                                                                        "end": 43
                                                                    },
                                                                    "flags": 512,
                                                                    "transformFlags": 0,
                                                                    "start": 23,
                                                                    "end": 43
                                                                }
                                                            ],
                                                            "flags": 32,
                                                            "transformFlags": 0,
                                                            "start": 23,
                                                            "end": 43
                                                        },
                                                        "flags": 21,
                                                        "transformFlags": 0,
                                                        "start": 32,
                                                        "end": 45
                                                    },
                                                    "flags": 16,
                                                    "transformFlags": 0,
                                                    "start": 13,
                                                    "end": 45
                                                }
                                            ],
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 13,
                                            "end": 45
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 11,
                                        "end": 45
                                    },
                                    "flags": 544,
                                    "transformFlags": 0,
                                    "start": 8,
                                    "end": 45
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 2,
                                "end": 45
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 2,
                        "end": 45
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 1,
                    "end": 45
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 0,
                "end": 46
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 46
        }
    ],
    "isModule": false,
    "source": "({ set x(_) { class C { set x(_) { super( } })",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 46
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ 'super' can only be referenced in members of derived classes or object literal expressions - start: 34, end: 41
✖ Expected a ')' to match the '(' token here - start: 42, end: 43
✖ The parser expected to find a '}' to match the '{' token here - start: 45, end: 46

```

