# Kataw parser test case

## Options

`````js
{ jsx: true, disableWebCompat: true }
`````

## Input

`````js
a().b
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
                "kind": 129,
                "member": {
                    "kind": 131,
                    "expression": {
                        "kind": 134299649,
                        "text": "a",
                        "rawText": "a",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 0,
                        "end": 1
                    },
                    "argumentList": {
                        "kind": 256,
                        "elements": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 2,
                        "end": 2
                    },
                    "flags": 32,
                    "transformFlags": 1,
                    "start": 0,
                    "end": 3
                },
                "expression": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 4,
                    "end": 5
                },
                "flags": 32,
                "transformFlags": 2,
                "start": 0,
                "end": 5
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 5
        }
    ],
    "isModule": false,
    "source": "a().b",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 5
}
```

### Printed

```javascript
a().b;
```

### Diagnostics

```javascript
✔ No errors
```

