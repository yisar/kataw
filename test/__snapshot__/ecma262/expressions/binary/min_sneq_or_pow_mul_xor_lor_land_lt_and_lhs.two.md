# Kataw parser test case

## Input

`````js
x0 - x1 !== x2 | x3 ** x4 * x5 ^ x6 || x7 && x8 < x9 & x10 << x
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
                "kind": 198,
                "left": {
                    "kind": 198,
                    "left": {
                        "kind": 198,
                        "left": {
                            "kind": 198,
                            "left": {
                                "kind": 134299649,
                                "text": "x0",
                                "rawText": "x0",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 0,
                                "end": 2
                            },
                            "operatorToken": {
                                "kind": 134318643,
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 2,
                                "end": 4
                            },
                            "right": {
                                "kind": 134299649,
                                "text": "x1",
                                "rawText": "x1",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 4,
                                "end": 7
                            },
                            "flags": 96,
                            "transformFlags": 5120,
                            "start": 0,
                            "end": 7
                        },
                        "operatorToken": {
                            "kind": 34621,
                            "flags": 96,
                            "transformFlags": 16,
                            "start": 7,
                            "end": 11
                        },
                        "right": {
                            "kind": 134299649,
                            "text": "x2",
                            "rawText": "x2",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 11,
                            "end": 14
                        },
                        "flags": 96,
                        "transformFlags": 5120,
                        "start": 0,
                        "end": 14
                    },
                    "operatorToken": {
                        "kind": 134251592,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 14,
                        "end": 16
                    },
                    "right": {
                        "kind": 198,
                        "left": {
                            "kind": 198,
                            "left": {
                                "kind": 198,
                                "left": {
                                    "kind": 134299649,
                                    "text": "x3",
                                    "rawText": "x3",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 16,
                                    "end": 19
                                },
                                "operatorToken": {
                                    "kind": 35897,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 19,
                                    "end": 22
                                },
                                "right": {
                                    "kind": 134299649,
                                    "text": "x4",
                                    "rawText": "x4",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 22,
                                    "end": 25
                                },
                                "flags": 96,
                                "transformFlags": 5120,
                                "start": 19,
                                "end": 25
                            },
                            "operatorToken": {
                                "kind": 201360950,
                                "flags": 96,
                                "transformFlags": 32,
                                "start": 25,
                                "end": 27
                            },
                            "right": {
                                "kind": 134299649,
                                "text": "x5",
                                "rawText": "x5",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 27,
                                "end": 30
                            },
                            "flags": 96,
                            "transformFlags": 5120,
                            "start": 19,
                            "end": 30
                        },
                        "operatorToken": {
                            "kind": 134251849,
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 30,
                            "end": 32
                        },
                        "right": {
                            "kind": 134299649,
                            "text": "x6",
                            "rawText": "x6",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 32,
                            "end": 35
                        },
                        "flags": 96,
                        "transformFlags": 5120,
                        "start": 19,
                        "end": 35
                    },
                    "flags": 96,
                    "transformFlags": 5120,
                    "start": 0,
                    "end": 35
                },
                "operatorToken": {
                    "kind": 33339,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 35,
                    "end": 38
                },
                "right": {
                    "kind": 198,
                    "left": {
                        "kind": 134299649,
                        "text": "x7",
                        "rawText": "x7",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 38,
                        "end": 41
                    },
                    "operatorToken": {
                        "kind": 33594,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 41,
                        "end": 44
                    },
                    "right": {
                        "kind": 198,
                        "left": {
                            "kind": 198,
                            "left": {
                                "kind": 134299649,
                                "text": "x8",
                                "rawText": "x8",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 44,
                                "end": 47
                            },
                            "operatorToken": {
                                "kind": 536971330,
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 47,
                                "end": 49
                            },
                            "right": {
                                "kind": 134299649,
                                "text": "x9",
                                "rawText": "x9",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 49,
                                "end": 52
                            },
                            "flags": 96,
                            "transformFlags": 5120,
                            "start": 47,
                            "end": 52
                        },
                        "operatorToken": {
                            "kind": 134252103,
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 52,
                            "end": 54
                        },
                        "right": {
                            "kind": 198,
                            "left": {
                                "kind": 134299649,
                                "text": "x10",
                                "rawText": "x10",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 54,
                                "end": 58
                            },
                            "operatorToken": {
                                "kind": 35140,
                                "flags": 96,
                                "transformFlags": 64,
                                "start": 58,
                                "end": 61
                            },
                            "right": {
                                "kind": 134299649,
                                "text": "x",
                                "rawText": "x",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 61,
                                "end": 63
                            },
                            "flags": 96,
                            "transformFlags": 5120,
                            "start": 58,
                            "end": 63
                        },
                        "flags": 96,
                        "transformFlags": 5120,
                        "start": 47,
                        "end": 63
                    },
                    "flags": 96,
                    "transformFlags": 5120,
                    "start": 41,
                    "end": 63
                },
                "flags": 96,
                "transformFlags": 5120,
                "start": 0,
                "end": 63
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 63
        }
    ],
    "isModule": false,
    "source": "x0 - x1 !== x2 | x3 ** x4 * x5 ^ x6 || x7 && x8 < x9 & x10 << x",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 63
}
```

### Printed

```javascript
x0 - x1 !== x2 | x3 ** x4 * x5 ^ x6 || x7 && x8  < x9 & x10 << x;
```

### Diagnostics

```javascript
✔ No errors
```

