# Kataw parser test case

## Input

`````js
var ];
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
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "declarationList": {
                "kind": 156,
                "declarations": [],
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 3
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 3
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 5,
            "end": 6
        }
    ],
    "isModule": false,
    "source": "var ];",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 6
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ ']' is not allowed here. Did you mean ';'? - start: 3, end: 5

```

