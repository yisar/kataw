# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/miscellaneous/destructuring/destructuring-assignment-positive-tests/autogen.md
- Path: kataw/test/__snapshot__/ecma262/miscellaneous/destructuring/destructuring-assignment-positive-tests/gen/var_and_for_in
> :: test: var and for in
> :: case: { import.meta }
## Options

`````js
{}
`````
## Input

`````js
var x, y, z; for (x in { import.meta } = z = {});
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
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "x",
                            "rawText": "x",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 5
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 3,
                        "end": 5
                    },
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "y",
                            "rawText": "y",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 6,
                            "end": 8
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 6,
                        "end": 8
                    },
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "z",
                            "rawText": "z",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 9,
                            "end": 11
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 9,
                        "end": 11
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 11
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 12
        },
        {
            "kind": 166,
            "forKeyword": {
                "kind": 37757017,
                "flags": 80,
                "transformFlags": 0,
                "start": 12,
                "end": 16
            },
            "initializer": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 18,
                "end": 19
            },
            "inKeyword": {
                "kind": 21006388,
                "flags": 64,
                "transformFlags": 0,
                "start": 19,
                "end": 22
            },
            "expression": {
                "kind": 129,
                "member": {
                    "kind": 220,
                    "propertyList": {
                        "kind": 218,
                        "properties": [
                            {
                                "kind": 134299649,
                                "text": "import",
                                "rawText": "import",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 24,
                                "end": 31
                            }
                        ],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 24,
                        "end": 31
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 22,
                    "end": 31
                },
                "expression": {
                    "kind": 134299649,
                    "text": "meta",
                    "rawText": "meta",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 32,
                    "end": 36
                },
                "flags": 48,
                "transformFlags": 2,
                "start": 22,
                "end": 36
            },
            "statement": {
                "kind": 120,
                "expression": {
                    "kind": 16637,
                    "text": "",
                    "rawText": "",
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 36,
                    "end": 36
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 36,
                "end": 36
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 12,
            "end": 36
        },
        {
            "kind": 120,
            "expression": {
                "kind": 125,
                "left": {
                    "kind": 134299649,
                    "text": "z",
                    "rawText": "z",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 40,
                    "end": 42
                },
                "operatorToken": {
                    "kind": 4125,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 42,
                    "end": 44
                },
                "right": {
                    "kind": 220,
                    "propertyList": {
                        "kind": 218,
                        "properties": [],
                        "trailingComma": false,
                        "flags": 16,
                        "transformFlags": 0,
                        "start": 46,
                        "end": 46
                    },
                    "flags": 48,
                    "transformFlags": 8,
                    "start": 44,
                    "end": 47
                },
                "flags": 0,
                "transformFlags": 128,
                "start": 40,
                "end": 47
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 40,
            "end": 47
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 48,
            "end": 49
        }
    ],
    "isModule": false,
    "source": "var x, y, z; for (x in { import.meta } = z = {});",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 49
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Property definition expected. Did you mean to use a ':'? - start: 31, end: 32
✖ ',' expected - start: 31, end: 32
✖ Expected a ')' to match the '(' token here - start: 37, end: 38
✖ Declaration or statement expected - start: 38, end: 40
✖ ')' is not allowed here. Did you mean ';'? - start: 47, end: 48

```

