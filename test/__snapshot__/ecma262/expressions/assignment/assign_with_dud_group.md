# Kataw parser test case

## Options

`````js
{ jsx: false, disableWebCompat: true }
`````

## Input

`````js
a = ((b)) = c;
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
                "kind": 125,
                "left": {
                    "kind": 134299649,
                    "text": "a",
                    "rawText": "a",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 0,
                    "end": 1
                },
                "operatorToken": {
                    "kind": 4125,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 1,
                    "end": 3
                },
                "right": {
                    "kind": 125,
                    "left": {
                        "kind": 121,
                        "expression": {
                            "kind": 121,
                            "expression": {
                                "kind": 134299649,
                                "text": "b",
                                "rawText": "b",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 6,
                                "end": 7
                            },
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 5,
                            "end": 8
                        },
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 3,
                        "end": 9
                    },
                    "operatorToken": {
                        "kind": 4125,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 9,
                        "end": 11
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "c",
                        "rawText": "c",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 11,
                        "end": 13
                    },
                    "flags": 0,
                    "transformFlags": 128,
                    "start": 3,
                    "end": 13
                },
                "flags": 0,
                "transformFlags": 128,
                "start": 0,
                "end": 13
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 14
        }
    ],
    "isModule": false,
    "source": "a = ((b)) = c;",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 14
}
```

### Printed

```javascript
a = ((b)) = c;
```

### Diagnostics

```javascript
✔ No errors
```

