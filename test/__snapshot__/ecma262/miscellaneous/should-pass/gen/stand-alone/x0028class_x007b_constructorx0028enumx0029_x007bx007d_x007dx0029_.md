# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/miscellaneous/should-pass/autogen.md
- Path: kataw/test/__snapshot__/ecma262/miscellaneous/should-pass/gen/stand-alone
> :: test: stand-alone
> :: case: (class { constructor(enum) {} });
## Options

`````js
{}
`````
## Input

`````js
(class { constructor(enum) {} });
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
                    "kind": 189,
                    "decorators": null,
                    "classKeyword": {
                        "kind": 37822544,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 6
                    },
                    "name": null,
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
                                    "getKeyword": null,
                                    "asteriskToken": null,
                                    "method": {
                                        "kind": 209,
                                        "name": {
                                            "kind": 134299649,
                                            "text": "constructor",
                                            "rawText": "constructor",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 8,
                                            "end": 20
                                        },
                                        "typeParameters": null,
                                        "formalParameterList": {
                                            "kind": 214,
                                            "formalParameters": [
                                                {
                                                    "kind": 134299649,
                                                    "text": "enum",
                                                    "rawText": "enum",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 21,
                                                    "end": 25
                                                }
                                            ],
                                            "trailingComma": false,
                                            "flags": 2144,
                                            "transformFlags": 0,
                                            "start": 21,
                                            "end": 26
                                        },
                                        "returnType": null,
                                        "contents": {
                                            "kind": 216,
                                            "functionStatementList": {
                                                "kind": 217,
                                                "directives": [],
                                                "statements": [],
                                                "flags": 32,
                                                "transformFlags": 0,
                                                "start": 28,
                                                "end": 28
                                            },
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 26,
                                            "end": 29
                                        },
                                        "flags": 2048,
                                        "transformFlags": 0,
                                        "start": 20,
                                        "end": 29
                                    },
                                    "flags": 2048,
                                    "transformFlags": 0,
                                    "start": 8,
                                    "end": 29
                                }
                            ],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 8,
                            "end": 29
                        },
                        "flags": 6,
                        "transformFlags": 0,
                        "start": 32,
                        "end": 31
                    },
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 1,
                    "end": 31
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 0,
                "end": 32
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 33
        }
    ],
    "isModule": false,
    "source": "(class { constructor(enum) {} });",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 33
}
```

### Printed

```javascript
(class {
    constructor(enum) {}
  });
```

### Diagnostics

```javascript
✔ No errors
```

