# Kataw parser test case

## Input

`````js
for ((x = y) in z) ;
`````

## Options

### Parser Options

`````js
{}
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 166,
            "forKeyword": {
                "kind": 37757017,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "initializer": {
                "kind": 121,
                "expression": {
                    "kind": 125,
                    "left": {
                        "kind": 134299649,
                        "text": "x",
                        "rawText": "x",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 6,
                        "end": 7
                    },
                    "operatorToken": {
                        "kind": 4125,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 7,
                        "end": 9
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "y",
                        "rawText": "y",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 9,
                        "end": 11
                    },
                    "flags": 32,
                    "transformFlags": 128,
                    "start": 5,
                    "end": 11
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 5,
                "end": 12
            },
            "inKeyword": {
                "kind": 21006388,
                "flags": 64,
                "transformFlags": 0,
                "start": 12,
                "end": 15
            },
            "expression": {
                "kind": 134299649,
                "text": "z",
                "rawText": "z",
                "flags": 96,
                "transformFlags": 0,
                "start": 15,
                "end": 17
            },
            "statement": {
                "kind": 168,
                "flags": 16,
                "transformFlags": 0,
                "start": 18,
                "end": 20
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 20
        }
    ],
    "isModule": false,
    "source": "for ((x = y) in z) ;",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 20
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ The left-hand side of a 'for...in' statement must be a variable or a property access. - start: 15, end: 17

```

