# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/binary/exponentiation-perator-errors/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/binary/exponentiation-perator-errors/gen/in_call_expression
> :: test: in call expression
> :: case: delete x ** 10
## Options

`````js
{}
`````
## Input

`````js
var O = { p: 1 }, x = 10; foo(delete x ** 10)
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "O",
                            "rawText": "O",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 5
                        },
                        "type": null,
                        "initializer": {
                            "kind": 220,
                            "propertyList": {
                                "kind": 218,
                                "properties": [
                                    {
                                        "kind": 219,
                                        "asteriskToken": null,
                                        "left": {
                                            "kind": 134299649,
                                            "text": "p",
                                            "rawText": "p",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 9,
                                            "end": 11
                                        },
                                        "right": {
                                            "kind": 201392130,
                                            "text": 1,
                                            "rawText": "1",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 12,
                                            "end": 14
                                        },
                                        "flags": 32,
                                        "transformFlags": 128,
                                        "start": 9,
                                        "end": 14
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 9,
                                "end": 14
                            },
                            "flags": 48,
                            "transformFlags": 8,
                            "start": 7,
                            "end": 16
                        },
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 3,
                        "end": 16
                    },
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "x",
                            "rawText": "x",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 17,
                            "end": 19
                        },
                        "type": null,
                        "initializer": {
                            "kind": 201392130,
                            "text": 10,
                            "rawText": "10",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 21,
                            "end": 24
                        },
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 17,
                        "end": 24
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 24
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 25
        },
        {
            "kind": 120,
            "expression": {
                "kind": 131,
                "expression": {
                    "kind": 134299649,
                    "text": "foo",
                    "rawText": "foo",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 25,
                    "end": 29
                },
                "argumentList": {
                    "kind": 256,
                    "elements": [
                        {
                            "kind": 198,
                            "left": {
                                "kind": 126,
                                "operandToken": {
                                    "kind": 4259886,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 30,
                                    "end": 36
                                },
                                "operand": {
                                    "kind": 134299649,
                                    "text": "x",
                                    "rawText": "x",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 36,
                                    "end": 38
                                },
                                "flags": 32,
                                "transformFlags": 16384,
                                "start": 30,
                                "end": 38
                            },
                            "operatorToken": {
                                "kind": 35897,
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 38,
                                "end": 41
                            },
                            "right": {
                                "kind": 201392130,
                                "text": 10,
                                "rawText": "10",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 41,
                                "end": 44
                            },
                            "flags": 32,
                            "transformFlags": 5120,
                            "start": 30,
                            "end": 44
                        }
                    ],
                    "trailingComma": false,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 30,
                    "end": 44
                },
                "flags": 32,
                "transformFlags": 1,
                "start": 25,
                "end": 45
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 25,
            "end": 45
        }
    ],
    "isModule": false,
    "source": "var O = { p: 1 }, x = 10; foo(delete x ** 10)",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 45
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Unary expressions as the left operand of an exponentation expression must be disambiguated with parentheses - start: 38, end: 41

```

