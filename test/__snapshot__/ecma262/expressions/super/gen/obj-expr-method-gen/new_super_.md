# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/super/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/super/gen/obj-expr-method-gen
> :: test: obj-expr-method-gen
> :: case: new super;
## Options

`````js
{}
`````
## Input

`````js
({ *method() { new super; } })
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
                                "asteriskToken": {
                                    "kind": 201360950,
                                    "flags": 64,
                                    "transformFlags": 32,
                                    "start": 2,
                                    "end": 4
                                },
                                "getKeyword": null,
                                "setKeyword": null,
                                "method": {
                                    "kind": 209,
                                    "name": {
                                        "kind": 134299649,
                                        "text": "method",
                                        "rawText": "method",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 4,
                                        "end": 10
                                    },
                                    "typeParameters": null,
                                    "formalParameterList": {
                                        "kind": 214,
                                        "formalParameters": [],
                                        "trailingComma": false,
                                        "flags": 160,
                                        "transformFlags": 0,
                                        "start": 11,
                                        "end": 12
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
                                                        "kind": 210,
                                                        "newKeyword": {
                                                            "kind": 138477661,
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 14,
                                                            "end": 18
                                                        },
                                                        "expression": {
                                                            "kind": 129,
                                                            "member": {
                                                                "kind": 4259935,
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 18,
                                                                "end": 24
                                                            },
                                                            "expression": {
                                                                "kind": 16637,
                                                                "text": "",
                                                                "rawText": "",
                                                                "flags": 64,
                                                                "transformFlags": 0,
                                                                "start": 24,
                                                                "end": 24
                                                            },
                                                            "flags": 32,
                                                            "transformFlags": 2,
                                                            "start": 18,
                                                            "end": 24
                                                        },
                                                        "argumentList": null,
                                                        "flags": 96,
                                                        "transformFlags": 2048,
                                                        "start": 14,
                                                        "end": 24
                                                    },
                                                    "flags": 16,
                                                    "transformFlags": 4096,
                                                    "start": 14,
                                                    "end": 25
                                                }
                                            ],
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 14,
                                            "end": 25
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 12,
                                        "end": 27
                                    },
                                    "flags": 160,
                                    "transformFlags": 0,
                                    "start": 10,
                                    "end": 27
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 2,
                                "end": 27
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 2,
                        "end": 27
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 1,
                    "end": 29
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 0,
                "end": 30
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 30
        }
    ],
    "isModule": false,
    "source": "({ *method() { new super; } })",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 30
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ 'super' must be followed by an argument list or member access. - start: 18, end: 25
✖ Dot property must be an identifier - start: 24, end: 25

```

