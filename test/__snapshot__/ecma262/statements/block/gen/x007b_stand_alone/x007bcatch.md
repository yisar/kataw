# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/block/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/block/gen/x007b_stand_alone
> :: test: { stand alone
> :: case: {catch
## Options

`````js
{}
`````
## Input

`````js
{ {catch
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
                            "statements": [
                                {
                                    "kind": 159,
                                    "tryKeyword": null,
                                    "block": {
                                        "kind": 124,
                                        "block": {
                                            "kind": 249,
                                            "statements": [],
                                            "flags": 16,
                                            "transformFlags": 0,
                                            "start": 3,
                                            "end": 3
                                        },
                                        "flags": 16,
                                        "transformFlags": 0,
                                        "start": 3,
                                        "end": 3
                                    },
                                    "catchClause": {
                                        "kind": 173,
                                        "catchKeyword": {
                                            "kind": 4202575,
                                            "flags": 80,
                                            "transformFlags": 0,
                                            "start": 3,
                                            "end": 8
                                        },
                                        "catchParameter": null,
                                        "block": {
                                            "kind": 124,
                                            "block": {
                                                "kind": 249,
                                                "statements": [],
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 8,
                                                "end": 8
                                            },
                                            "flags": 16,
                                            "transformFlags": 0,
                                            "start": 8,
                                            "end": 8
                                        },
                                        "flags": 80,
                                        "transformFlags": 0,
                                        "start": 3,
                                        "end": 8
                                    },
                                    "finallyKeyword": null,
                                    "finallyBlock": null,
                                    "flags": 16,
                                    "transformFlags": 0,
                                    "start": 3,
                                    "end": 8
                                }
                            ],
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 8
                        },
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 8
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 1,
                "end": 8
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 8
        }
    ],
    "isModule": false,
    "source": "{ {catch",
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
✖ The parser expected to find a '}' to match the '{' token here - start: 3, end: 8

```

