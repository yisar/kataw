# Kataw parser test case

## Input

`````js
for (const x = y;;) { var x; }
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 165,
            "forKeyword": {
                "kind": 37757017,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "initializer": {
                "kind": 162,
                "lexicalKeyword": {
                    "kind": 37757004,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 5,
                    "end": 10
                },
                "binding": {
                    "kind": 151,
                    "bindingList": [
                        {
                            "kind": 190,
                            "binding": {
                                "kind": 134299649,
                                "text": "x",
                                "rawText": "x",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 10,
                                "end": 12
                            },
                            "type": null,
                            "initializer": {
                                "kind": 134299649,
                                "text": "y",
                                "rawText": "y",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 14,
                                "end": 16
                            },
                            "flags": 16,
                            "transformFlags": 4224,
                            "start": 10,
                            "end": 16
                        }
                    ],
                    "flags": 16777232,
                    "transformFlags": 0,
                    "start": 10,
                    "end": 16
                },
                "flags": 33554448,
                "transformFlags": 0,
                "start": 0,
                "end": 16
            },
            "condition": null,
            "incrementor": null,
            "statement": {
                "kind": 124,
                "block": {
                    "kind": 249,
                    "statements": [
                        {
                            "kind": 155,
                            "declareKeyword": null,
                            "varKeyword": {
                                "kind": 37757002,
                                "flags": 80,
                                "transformFlags": 0,
                                "start": 21,
                                "end": 25
                            },
                            "declarationList": {
                                "kind": 156,
                                "declarations": [
                                    {
                                        "kind": 157,
                                        "binding": {
                                            "kind": 134299649,
                                            "text": "x",
                                            "rawText": "x",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 25,
                                            "end": 27
                                        },
                                        "type": null,
                                        "initializer": null,
                                        "flags": 16,
                                        "transformFlags": 4224,
                                        "start": 25,
                                        "end": 27
                                    }
                                ],
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 25,
                                "end": 27
                            },
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 21,
                            "end": 28
                        }
                    ],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 21,
                    "end": 28
                },
                "flags": 16,
                "transformFlags": 0,
                "start": 19,
                "end": 30
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 30
        }
    ],
    "isModule": false,
    "source": "for (const x = y;;) { var x; }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 30
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Cannot redeclare block-scoped variable 'x' - start: 25, end: 27

```

