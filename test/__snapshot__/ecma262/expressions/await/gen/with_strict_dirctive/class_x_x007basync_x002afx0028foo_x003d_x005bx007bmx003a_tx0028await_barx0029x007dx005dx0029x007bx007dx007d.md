# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/await/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/await/gen/with_strict_dirctive
> :: test: with_strict_dirctive
> :: case: class x {async *f(foo = [{m: t(await bar)}]){}}
## Options

`````js
{}
`````
## Input

`````js
'use strict'; class x {async *f(foo = [{m: t(await bar)}]){}}
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [
        {
            "kind": 201392131,
            "text": "use strict",
            "rawText": "'use strict'",
            "flags": 4194400,
            "transformFlags": 0,
            "start": 0,
            "end": 12
        }
    ],
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
                "text": "x",
                "rawText": "x",
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
                            "asyncKeyword": {
                                "kind": 82031,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 23,
                                "end": 28
                            },
                            "setKeyword": null,
                            "getKeyword": null,
                            "asteriskToken": {
                                "kind": 201360950,
                                "flags": 64,
                                "transformFlags": 32,
                                "start": 28,
                                "end": 30
                            },
                            "method": {
                                "kind": 209,
                                "name": {
                                    "kind": 134299649,
                                    "text": "f",
                                    "rawText": "f",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 30,
                                    "end": 31
                                },
                                "typeParameters": null,
                                "formalParameterList": {
                                    "kind": 214,
                                    "formalParameters": [
                                        {
                                            "kind": 281,
                                            "ellipsisToken": null,
                                            "left": {
                                                "kind": 134299649,
                                                "text": "foo",
                                                "rawText": "foo",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 32,
                                                "end": 35
                                            },
                                            "optionalToken": null,
                                            "type": null,
                                            "right": {
                                                "kind": 119,
                                                "elementList": {
                                                    "kind": 270,
                                                    "elements": [
                                                        {
                                                            "kind": 220,
                                                            "propertyList": {
                                                                "kind": 218,
                                                                "properties": [
                                                                    {
                                                                        "kind": 219,
                                                                        "asteriskToken": null,
                                                                        "left": {
                                                                            "kind": 134299649,
                                                                            "text": "m",
                                                                            "rawText": "m",
                                                                            "flags": 96,
                                                                            "transformFlags": 0,
                                                                            "start": 40,
                                                                            "end": 41
                                                                        },
                                                                        "right": {
                                                                            "kind": 131,
                                                                            "expression": {
                                                                                "kind": 134299649,
                                                                                "text": "t",
                                                                                "rawText": "t",
                                                                                "flags": 96,
                                                                                "transformFlags": 0,
                                                                                "start": 42,
                                                                                "end": 44
                                                                            },
                                                                            "argumentList": {
                                                                                "kind": 256,
                                                                                "elements": [
                                                                                    {
                                                                                        "kind": 208,
                                                                                        "awaitKeyword": {
                                                                                            "kind": 82196,
                                                                                            "flags": 64,
                                                                                            "transformFlags": 0,
                                                                                            "start": 45,
                                                                                            "end": 50
                                                                                        },
                                                                                        "expression": {
                                                                                            "kind": 134299649,
                                                                                            "text": "bar",
                                                                                            "rawText": "bar",
                                                                                            "flags": 96,
                                                                                            "transformFlags": 0,
                                                                                            "start": 50,
                                                                                            "end": 54
                                                                                        },
                                                                                        "flags": 32,
                                                                                        "transformFlags": 4096,
                                                                                        "start": 45,
                                                                                        "end": 54
                                                                                    }
                                                                                ],
                                                                                "trailingComma": false,
                                                                                "flags": 32,
                                                                                "transformFlags": 0,
                                                                                "start": 45,
                                                                                "end": 54
                                                                            },
                                                                            "flags": 32,
                                                                            "transformFlags": 1,
                                                                            "start": 40,
                                                                            "end": 55
                                                                        },
                                                                        "flags": 32,
                                                                        "transformFlags": 128,
                                                                        "start": 40,
                                                                        "end": 55
                                                                    }
                                                                ],
                                                                "trailingComma": false,
                                                                "flags": 16,
                                                                "transformFlags": 0,
                                                                "start": 40,
                                                                "end": 55
                                                            },
                                                            "flags": 48,
                                                            "transformFlags": 8,
                                                            "start": 39,
                                                            "end": 56
                                                        }
                                                    ],
                                                    "trailingComma": false,
                                                    "flags": 32,
                                                    "transformFlags": 0,
                                                    "start": 39,
                                                    "end": 56
                                                },
                                                "flags": 32,
                                                "transformFlags": 8,
                                                "start": 37,
                                                "end": 57
                                            },
                                            "flags": 34,
                                            "transformFlags": 4096,
                                            "start": 32,
                                            "end": 57
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 418,
                                    "transformFlags": 0,
                                    "start": 32,
                                    "end": 58
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
                                        "start": 59,
                                        "end": 59
                                    },
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 58,
                                    "end": 60
                                },
                                "flags": 384,
                                "transformFlags": 0,
                                "start": 31,
                                "end": 60
                            },
                            "flags": 384,
                            "transformFlags": 0,
                            "start": 23,
                            "end": 60
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 23,
                    "end": 60
                },
                "flags": 21,
                "transformFlags": 0,
                "start": 32,
                "end": 61
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 13,
            "end": 61
        }
    ],
    "isModule": false,
    "source": "'use strict'; class x {async *f(foo = [{m: t(await bar)}]){}}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 61
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ `await` expression cannot be used in function parameters - start: 45, end: 50

```

