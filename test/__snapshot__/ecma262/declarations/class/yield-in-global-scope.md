# Kataw parser test case

## Input

`````js
yield 10
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
                "text": "yield",
                "rawText": "yield",
                "flags": 96,
                "transformFlags": 0,
                "start": 0,
                "end": 5
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 5
        },
        {
            "kind": 120,
            "expression": {
                "kind": 201392130,
                "text": 10,
                "rawText": "10",
                "flags": 96,
                "transformFlags": 0,
                "start": 5,
                "end": 8
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 5,
            "end": 8
        }
    ],
    "isModule": false,
    "source": "yield 10",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 8
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ '; ' is not allowed here. Did you mean ';'? - start: 5, end: 8

```

