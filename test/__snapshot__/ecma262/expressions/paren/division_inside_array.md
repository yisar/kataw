# Kataw parser test case

## Input

`````js
([a / b]);

([a / b], ([a / b]));
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
                    "kind": 119,
                    "elementList": {
                        "kind": 270,
                        "elements": [
                            {
                                "kind": 198,
                                "left": {
                                    "kind": 134299649,
                                    "text": "a",
                                    "rawText": "a",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 2,
                                    "end": 3
                                },
                                "operatorToken": {
                                    "kind": 35640,
                                    "flags": 96,
                                    "transformFlags": 32,
                                    "start": 3,
                                    "end": 5
                                },
                                "right": {
                                    "kind": 134299649,
                                    "text": "b",
                                    "rawText": "b",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 5,
                                    "end": 7
                                },
                                "flags": 96,
                                "transformFlags": 5120,
                                "start": 2,
                                "end": 7
                            }
                        ],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 2,
                        "end": 7
                    },
                    "flags": 32,
                    "transformFlags": 8,
                    "start": 1,
                    "end": 8
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 0,
                "end": 9
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 10
        },
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 132,
                    "expressions": [
                        {
                            "kind": 119,
                            "elementList": {
                                "kind": 270,
                                "elements": [
                                    {
                                        "kind": 198,
                                        "left": {
                                            "kind": 134299649,
                                            "text": "a",
                                            "rawText": "a",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 14,
                                            "end": 15
                                        },
                                        "operatorToken": {
                                            "kind": 35640,
                                            "flags": 96,
                                            "transformFlags": 32,
                                            "start": 15,
                                            "end": 17
                                        },
                                        "right": {
                                            "kind": 134299649,
                                            "text": "b",
                                            "rawText": "b",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 17,
                                            "end": 19
                                        },
                                        "flags": 96,
                                        "transformFlags": 5120,
                                        "start": 14,
                                        "end": 19
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 14,
                                "end": 19
                            },
                            "flags": 32,
                            "transformFlags": 8,
                            "start": 13,
                            "end": 20
                        },
                        {
                            "kind": 121,
                            "expression": {
                                "kind": 119,
                                "elementList": {
                                    "kind": 270,
                                    "elements": [
                                        {
                                            "kind": 198,
                                            "left": {
                                                "kind": 134299649,
                                                "text": "a",
                                                "rawText": "a",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 24,
                                                "end": 25
                                            },
                                            "operatorToken": {
                                                "kind": 35640,
                                                "flags": 96,
                                                "transformFlags": 32,
                                                "start": 25,
                                                "end": 27
                                            },
                                            "right": {
                                                "kind": 134299649,
                                                "text": "b",
                                                "rawText": "b",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 27,
                                                "end": 29
                                            },
                                            "flags": 96,
                                            "transformFlags": 5120,
                                            "start": 24,
                                            "end": 29
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 24,
                                    "end": 29
                                },
                                "flags": 32,
                                "transformFlags": 8,
                                "start": 23,
                                "end": 30
                            },
                            "flags": 34,
                            "transformFlags": 0,
                            "start": 21,
                            "end": 31
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 1024,
                    "start": 10,
                    "end": 31
                },
                "flags": 35,
                "transformFlags": 0,
                "start": 10,
                "end": 32
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 10,
            "end": 33
        }
    ],
    "isModule": false,
    "source": "([a / b]);\n\n([a / b], ([a / b]));",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 33
}
```

### Printed

```javascript
([a / b]);
([a / b], ([a / b]));

```

### Diagnostics

```javascript
✔ No errors
```

