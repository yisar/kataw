# Kataw parser test case

## Input

`````js
(foo + (bar + boo) + ding)
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
                    "kind": 198,
                    "left": {
                        "kind": 198,
                        "left": {
                            "kind": 134299649,
                            "text": "foo",
                            "rawText": "foo",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 1,
                            "end": 4
                        },
                        "operatorToken": {
                            "kind": 99634,
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 4,
                            "end": 6
                        },
                        "right": {
                            "kind": 121,
                            "expression": {
                                "kind": 198,
                                "left": {
                                    "kind": 134299649,
                                    "text": "bar",
                                    "rawText": "bar",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 8,
                                    "end": 11
                                },
                                "operatorToken": {
                                    "kind": 99634,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 11,
                                    "end": 13
                                },
                                "right": {
                                    "kind": 134299649,
                                    "text": "boo",
                                    "rawText": "boo",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 13,
                                    "end": 17
                                },
                                "flags": 96,
                                "transformFlags": 5120,
                                "start": 6,
                                "end": 17
                            },
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 6,
                            "end": 18
                        },
                        "flags": 96,
                        "transformFlags": 5120,
                        "start": 0,
                        "end": 18
                    },
                    "operatorToken": {
                        "kind": 99634,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 18,
                        "end": 20
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "ding",
                        "rawText": "ding",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 20,
                        "end": 25
                    },
                    "flags": 96,
                    "transformFlags": 5120,
                    "start": 0,
                    "end": 25
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 0,
                "end": 26
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 26
        }
    ],
    "isModule": false,
    "source": "(foo + (bar + boo) + ding)",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 26
}
```

### Printed

```javascript
(foo + (bar + boo) + ding);
```

### Diagnostics

```javascript
✔ No errors
```

