# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/await/async-await-errors/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/await/async-await-errors/gen/with_strict_directive
> :: test: with strict directive
> :: case: ar O = { async method(x = await 1) { return x; } };
## Options

`````js
{}
`````
## Input

`````js
'use strict'; ar O = { async method(x = await 1) { return x; } };
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
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "ar",
                "rawText": "ar",
                "flags": 96,
                "transformFlags": 0,
                "start": 13,
                "end": 16
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 13,
            "end": 16
        },
        {
            "kind": 120,
            "expression": {
                "kind": 125,
                "left": {
                    "kind": 134299649,
                    "text": "O",
                    "rawText": "O",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 16,
                    "end": 18
                },
                "operatorToken": {
                    "kind": 4125,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 18,
                    "end": 20
                },
                "right": {
                    "kind": 220,
                    "propertyList": {
                        "kind": 218,
                        "properties": [
                            {
                                "kind": 351,
                                "asyncKeyword": {
                                    "kind": 82031,
                                    "flags": 352,
                                    "transformFlags": 0,
                                    "start": 22,
                                    "end": 28
                                },
                                "asteriskToken": null,
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
                                        "start": 28,
                                        "end": 35
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
                                                    "text": "x",
                                                    "rawText": "x",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 36,
                                                    "end": 37
                                                },
                                                "optionalToken": null,
                                                "type": null,
                                                "right": {
                                                    "kind": 208,
                                                    "awaitKeyword": {
                                                        "kind": 82196,
                                                        "flags": 64,
                                                        "transformFlags": 0,
                                                        "start": 39,
                                                        "end": 45
                                                    },
                                                    "expression": {
                                                        "kind": 201392130,
                                                        "text": 1,
                                                        "rawText": "1",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 45,
                                                        "end": 47
                                                    },
                                                    "flags": 32,
                                                    "transformFlags": 4096,
                                                    "start": 39,
                                                    "end": 47
                                                },
                                                "flags": 34,
                                                "transformFlags": 4096,
                                                "start": 36,
                                                "end": 47
                                            }
                                        ],
                                        "trailingComma": false,
                                        "flags": 290,
                                        "transformFlags": 0,
                                        "start": 36,
                                        "end": 48
                                    },
                                    "returnType": null,
                                    "contents": {
                                        "kind": 216,
                                        "functionStatementList": {
                                            "kind": 217,
                                            "directives": [],
                                            "statements": [
                                                {
                                                    "kind": 161,
                                                    "returnKeyword": {
                                                        "kind": 37757022,
                                                        "flags": 80,
                                                        "transformFlags": 0,
                                                        "start": 50,
                                                        "end": 57
                                                    },
                                                    "expression": {
                                                        "kind": 134299649,
                                                        "text": "x",
                                                        "rawText": "x",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 57,
                                                        "end": 59
                                                    },
                                                    "flags": 80,
                                                    "transformFlags": 256,
                                                    "start": 50,
                                                    "end": 60
                                                }
                                            ],
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 50,
                                            "end": 60
                                        },
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 48,
                                        "end": 62
                                    },
                                    "flags": 288,
                                    "transformFlags": 0,
                                    "start": 35,
                                    "end": 62
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 22,
                                "end": 62
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 22,
                        "end": 62
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 20,
                    "end": 64
                },
                "flags": 0,
                "transformFlags": 128,
                "start": 16,
                "end": 64
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 16,
            "end": 65
        }
    ],
    "isModule": false,
    "source": "'use strict'; ar O = { async method(x = await 1) { return x; } };",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 65
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ '; ' is not allowed here. Did you mean ';'? - start: 16, end: 18
✖ `await` expression cannot be used in function parameters - start: 39, end: 45

```

