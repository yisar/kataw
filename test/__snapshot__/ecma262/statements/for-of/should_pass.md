# Kataw parser test case

## Input

`````js
for ({[a]: ""[b] = c} of d) {}
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 167,
            "forKeyword": {
                "kind": 37757017,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "awaitKeyword": null,
            "initializer": {
                "kind": 220,
                "propertyList": {
                    "kind": 218,
                    "properties": [
                        {
                            "kind": 219,
                            "asteriskToken": null,
                            "left": {
                                "kind": 194,
                                "expression": {
                                    "kind": 134299649,
                                    "text": "a",
                                    "rawText": "a",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 7,
                                    "end": 8
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 6,
                                "end": 9
                            },
                            "right": {
                                "kind": 125,
                                "left": {
                                    "kind": 130,
                                    "member": {
                                        "kind": 201392131,
                                        "text": "",
                                        "rawText": "\"\"",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 10,
                                        "end": 13
                                    },
                                    "expression": {
                                        "kind": 134299649,
                                        "text": "b",
                                        "rawText": "b",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 14,
                                        "end": 15
                                    },
                                    "flags": 32,
                                    "transformFlags": 4,
                                    "start": 10,
                                    "end": 16
                                },
                                "operatorToken": {
                                    "kind": 4125,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 16,
                                    "end": 18
                                },
                                "right": {
                                    "kind": 134299649,
                                    "text": "c",
                                    "rawText": "c",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 18,
                                    "end": 20
                                },
                                "flags": 32,
                                "transformFlags": 128,
                                "start": 6,
                                "end": 20
                            },
                            "flags": 32,
                            "transformFlags": 128,
                            "start": 6,
                            "end": 20
                        }
                    ],
                    "trailingComma": false,
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 6,
                    "end": 20
                },
                "flags": 48,
                "transformFlags": 8,
                "start": 5,
                "end": 21
            },
            "ofKeyword": {
                "kind": 16793717,
                "flags": 64,
                "transformFlags": 0,
                "start": 21,
                "end": 24
            },
            "expression": {
                "kind": 134299649,
                "text": "d",
                "rawText": "d",
                "flags": 96,
                "transformFlags": 0,
                "start": 24,
                "end": 26
            },
            "statement": {
                "kind": 124,
                "block": {
                    "kind": 249,
                    "statements": [],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 29,
                    "end": 29
                },
                "flags": 16,
                "transformFlags": 0,
                "start": 27,
                "end": 30
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 30
        }
    ],
    "isModule": false,
    "source": "for ({[a]: \"\"[b] = c} of d) {}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 30
}
```

### Printed

```javascript
for ({ [a]: "\"\""[b] = c } of d) {}
```

### Diagnostics

```javascript
✔ No errors
```

