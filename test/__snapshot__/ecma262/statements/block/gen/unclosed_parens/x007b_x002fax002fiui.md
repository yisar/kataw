# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/block/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/block/gen/unclosed_parens
> :: test: unclosed parens
> :: case: { /a/iui
## Options

`````js
{}
`````
## Input

`````js
{( { /a/iui
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
                            "kind": 121,
                            "expression": {
                                "kind": 132,
                                "expressions": [],
                                "flags": 32,
                                "transformFlags": 1024,
                                "start": 1,
                                "end": 4
                            },
                            "flags": 34,
                            "transformFlags": 0,
                            "start": 1,
                            "end": 4
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 1,
                        "end": 4
                    },
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 371,
                            "text": "/a/iui",
                            "rawText": "/a/iui",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 4,
                            "end": 11
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 4,
                        "end": 11
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 1,
                "end": 11
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 11
        }
    ],
    "isModule": false,
    "source": "{( { /a/iui",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 11
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Duplicate regular expression flag - start: 9, end: 10
✖ The parser expected to find a '}' to match the '{' token here - start: 5, end: 11

```

