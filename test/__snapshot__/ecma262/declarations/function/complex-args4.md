# Kataw parser test case

## Input

`````js
unction f([b, a], ...b) {}
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
                "kind": 134299649,
                "text": "unction",
                "rawText": "unction",
                "flags": 96,
                "transformFlags": 0,
                "start": 0,
                "end": 7
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 7
        },
        {
            "kind": 120,
            "expression": {
                "kind": 131,
                "expression": {
                    "kind": 134299649,
                    "text": "f",
                    "rawText": "f",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 7,
                    "end": 9
                },
                "argumentList": {
                    "kind": 256,
                    "elements": [
                        {
                            "kind": 119,
                            "elementList": {
                                "kind": 270,
                                "elements": [
                                    {
                                        "kind": 134299649,
                                        "text": "b",
                                        "rawText": "b",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 11,
                                        "end": 12
                                    },
                                    {
                                        "kind": 134299649,
                                        "text": "a",
                                        "rawText": "a",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 13,
                                        "end": 15
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 11,
                                "end": 15
                            },
                            "flags": 32,
                            "transformFlags": 8,
                            "start": 10,
                            "end": 16
                        },
                        {
                            "kind": 223,
                            "ellipsisToken": {
                                "kind": 524302,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 17,
                                "end": 21
                            },
                            "argument": {
                                "kind": 134299649,
                                "text": "b",
                                "rawText": "b",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 21,
                                "end": 22
                            },
                            "flags": 1073741856,
                            "transformFlags": 0,
                            "start": 17,
                            "end": 22
                        }
                    ],
                    "trailingComma": false,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 10,
                    "end": 22
                },
                "flags": 32,
                "transformFlags": 1,
                "start": 7,
                "end": 23
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 7,
            "end": 23
        },
        {
            "kind": 124,
            "block": {
                "kind": 249,
                "statements": [],
                "flags": 16,
                "transformFlags": 0,
                "start": 25,
                "end": 25
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 23,
            "end": 26
        }
    ],
    "isModule": false,
    "source": "unction f([b, a], ...b) {}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 26
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ '; ' is not allowed here. Did you mean ';'? - start: 7, end: 9
✖ '{' is not allowed here. Did you mean ';'? - start: 23, end: 25

```

