# Kataw parser test case

## Options

`````js
{ jsx: false, disableWebCompat: true, module: true }
`````


## Input

`````js
({...{x} /= y});
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
                "kind": 121,
                "expression": {
                    "kind": 220,
                    "propertyList": {
                        "kind": 218,
                        "properties": [
                            {
                                "kind": 224,
                                "ellipsisToken": {
                                    "kind": 524302,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 2,
                                    "end": 5
                                },
                                "argument": {
                                    "kind": 125,
                                    "left": {
                                        "kind": 220,
                                        "propertyList": {
                                            "kind": 218,
                                            "properties": [
                                                {
                                                    "kind": 134299649,
                                                    "text": "x",
                                                    "rawText": "x",
                                                    "flags": 96,
                                                    "transformFlags": 0,
                                                    "start": 6,
                                                    "end": 7
                                                }
                                            ],
                                            "trailingComma": false,
                                            "flags": 16,
                                            "transformFlags": 0,
                                            "start": 6,
                                            "end": 7
                                        },
                                        "flags": 48,
                                        "transformFlags": 8,
                                        "start": 5,
                                        "end": 8
                                    },
                                    "operatorToken": {
                                        "kind": 4133,
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 8,
                                        "end": 11
                                    },
                                    "right": {
                                        "kind": 134299649,
                                        "text": "y",
                                        "rawText": "y",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 11,
                                        "end": 13
                                    },
                                    "flags": 32,
                                    "transformFlags": 128,
                                    "start": 5,
                                    "end": 13
                                },
                                "flags": 1073741856,
                                "transformFlags": 0,
                                "start": 2,
                                "end": 13
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 2,
                        "end": 13
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 1,
                    "end": 14
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 0,
                "end": 15
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 16
        }
    ],
    "isModule": true,
    "source": "({...{x} /= y});",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 16
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Expression exprected. A compound assignment or an logical assignment cannot follow an object literal - start: 5, end: 11

```

