# Kataw parser test case

## Input

`````js
foo(a)(b)(c)(d)(e)
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
                    "kind": 131,
                    "expression": {
                        "kind": 131,
                        "expression": {
                            "kind": 131,
                            "expression": {
                                "kind": 131,
                                "expression": {
                                    "kind": 134299649,
                                    "text": "foo",
                                    "rawText": "foo",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 0,
                                    "end": 3
                                },
                                "argumentList": {
                                    "kind": 256,
                                    "elements": [
                                        {
                                            "kind": 134299649,
                                            "text": "a",
                                            "rawText": "a",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 4,
                                            "end": 5
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 4,
                                    "end": 5
                                },
                                "flags": 32,
                                "transformFlags": 1,
                                "start": 0,
                                "end": 6
                            },
                            "argumentList": {
                                "kind": 256,
                                "elements": [
                                    {
                                        "kind": 134299649,
                                        "text": "b",
                                        "rawText": "b",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 7,
                                        "end": 8
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 7,
                                "end": 8
                            },
                            "flags": 32,
                            "transformFlags": 1,
                            "start": 0,
                            "end": 9
                        },
                        "argumentList": {
                            "kind": 256,
                            "elements": [
                                {
                                    "kind": 134299649,
                                    "text": "c",
                                    "rawText": "c",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 10,
                                    "end": 11
                                }
                            ],
                            "trailingComma": false,
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 10,
                            "end": 11
                        },
                        "flags": 32,
                        "transformFlags": 1,
                        "start": 0,
                        "end": 12
                    },
                    "argumentList": {
                        "kind": 256,
                        "elements": [
                            {
                                "kind": 134299649,
                                "text": "d",
                                "rawText": "d",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 13,
                                "end": 14
                            }
                        ],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 13,
                        "end": 14
                    },
                    "flags": 32,
                    "transformFlags": 1,
                    "start": 0,
                    "end": 15
                },
                "argumentList": {
                    "kind": 256,
                    "elements": [
                        {
                            "kind": 134299649,
                            "text": "e",
                            "rawText": "e",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 16,
                            "end": 17
                        }
                    ],
                    "trailingComma": false,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 16,
                    "end": 17
                },
                "flags": 32,
                "transformFlags": 1,
                "start": 0,
                "end": 18
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 18
        }
    ],
    "isModule": false,
    "source": "foo(a)(b)(c)(d)(e)",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 18
}
```

### Printed

```javascript
foo(a)(b)(c)(d)(e);
```

### Diagnostics

```javascript
✔ No errors
```

