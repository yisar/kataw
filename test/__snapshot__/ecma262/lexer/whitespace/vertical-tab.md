# Kataw parser test case

## Options

`````js
{ jsx: false, disableWebCompat: true }
`````

## Input

`````js
left|right
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
                    "kind": 134299649,
                    "text": "left",
                    "rawText": "left",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 0,
                    "end": 4
                },
                "operatorToken": {
                    "kind": 134251592,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 4,
                    "end": 5
                },
                "right": {
                    "kind": 134299649,
                    "text": "right",
                    "rawText": "right",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 5,
                    "end": 10
                },
                "flags": 96,
                "transformFlags": 5120,
                "start": 0,
                "end": 10
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 10
        }
    ],
    "isModule": false,
    "source": "left|right",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 10
}
```

### Printed

```javascript
left | right;
```

### Diagnostics

```javascript
✔ No errors
```

