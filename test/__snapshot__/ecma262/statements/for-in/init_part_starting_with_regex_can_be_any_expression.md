# Kataw parser test case

## Input

`````js
for (/x/g + b in obj);
`````

## Options

### Parser Options

`````js
{}
`````

### Printer Options

`````js
{
  "tabWidth": 2,
  "printWidth": 80,
  "useTabs": false,
  "bracketSpacing": true
}
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
                "kind": 198,
                "left": {
                    "kind": 371,
                    "text": "/x/g",
                    "rawText": "/x/g",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 5,
                    "end": 9
                },
                "operatorToken": {
                    "kind": 99634,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 9,
                    "end": 11
                },
                "right": {
                    "kind": 198,
                    "left": {
                        "kind": 134299649,
                        "text": "b",
                        "rawText": "b",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 11,
                        "end": 13
                    },
                    "operatorToken": {
                        "kind": 21006388,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 13,
                        "end": 16
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "obj",
                        "rawText": "obj",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 16,
                        "end": 20
                    },
                    "flags": 96,
                    "transformFlags": 5120,
                    "start": 13,
                    "end": 20
                },
                "flags": 96,
                "transformFlags": 5120,
                "start": 0,
                "end": 20
            },
            "condition": null,
            "incrementor": {
                "kind": 16637,
                "text": "",
                "rawText": "",
                "flags": 64,
                "transformFlags": 0,
                "start": 20,
                "end": 20
            },
            "statement": {
                "kind": 168,
                "flags": 16,
                "transformFlags": 0,
                "start": 21,
                "end": 22
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 22
        }
    ],
    "isModule": false,
    "source": "for (/x/g + b in obj);",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 22
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Identifier expected - start: 20, end: 21

```

