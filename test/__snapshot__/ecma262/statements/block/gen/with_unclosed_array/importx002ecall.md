# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/block/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/block/gen/with_unclosed_array
> :: test: with unclosed array
> :: case: import.call
## Options

`````js
{}
`````
## Input

`````js
{[ import.call
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 124,
            "block": {
                "kind": 249,
                "statements": [
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 119,
                            "elementList": {
                                "kind": 270,
                                "elements": [
                                    {
                                        "kind": 299,
                                        "importKeyword": {
                                            "kind": 37814364,
                                            "flags": 64,
                                            "transformFlags": 0,
                                            "start": 2,
                                            "end": 9
                                        },
                                        "metaIdentifier": null,
                                        "flags": 9,
                                        "transformFlags": 0,
                                        "start": 96,
                                        "end": 10
                                    },
                                    {
                                        "kind": 134299649,
                                        "text": "call",
                                        "rawText": "call",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 10,
                                        "end": 14
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 2,
                                "end": 14
                            },
                            "flags": 32,
                            "transformFlags": 8,
                            "start": 1,
                            "end": 14
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 1,
                        "end": 14
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 1,
                "end": 14
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 14
        }
    ],
    "isModule": false,
    "source": "{[ import.call",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 14
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Cannot use 'import.meta' outside a module - start: 9, end: 14
✖ 'import.meta' is the only valid meta property for import - start: 9, end: 14
✖ ',' expected - start: 10, end: 14

```

