# Kataw parser test case

## Input

`````js
bar ? (=> 0) : baz;
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
                "kind": 197,
                "shortCircuit": {
                    "kind": 134299649,
                    "text": "bar",
                    "rawText": "bar",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 0,
                    "end": 3
                },
                "questionToken": {
                    "kind": 134217750,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 3,
                    "end": 5
                },
                "consequent": {
                    "kind": 121,
                    "expression": {
                        "kind": 16637,
                        "text": "",
                        "rawText": "",
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 7,
                        "end": 7
                    },
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 5,
                    "end": 7
                },
                "colonToken": null,
                "alternate": {
                    "kind": 16637,
                    "text": "",
                    "rawText": "",
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 7,
                    "end": 7
                },
                "flags": 96,
                "transformFlags": 4096,
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
                "kind": 201392130,
                "text": 0,
                "rawText": "0",
                "flags": 96,
                "transformFlags": 0,
                "start": 9,
                "end": 11
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 9,
            "end": 11
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "baz",
                "rawText": "baz",
                "flags": 96,
                "transformFlags": 0,
                "start": 14,
                "end": 18
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 14,
            "end": 19
        }
    ],
    "isModule": false,
    "source": "bar ? (=> 0) : baz;",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 19
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Identifier expected - start: 7, end: 9
✖ Arrow parameters can only contain a binding pattern or an identifier - start: 5, end: 9
✖ ')' is not allowed here. Did you mean ';'? - start: 11, end: 12
✖ Declaration or statement expected - start: 12, end: 14

```

