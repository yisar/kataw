# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/block/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/block/gen/missing_parens_and_block
> :: test: missing parens and block
> :: case: as = x
## Options

`````js
{}
`````
## Input

`````js
{{
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
                        "kind": 124,
                        "block": {
                            "kind": 249,
                            "statements": [],
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 2,
                            "end": 2
                        },
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 2
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 1,
                "end": 2
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 2
        }
    ],
    "isModule": false,
    "source": "{{",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 2
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ The parser expected to find a '}' to match the '{' token here - start: 1, end: 2

```

