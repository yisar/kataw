# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/declarations/let/sub-tree/autogen.md
- Path: kataw/test/__snapshot__/ecma262/declarations/let/sub-tree/gen/if_else
> :: test: if else
> :: case: let {x}
## Options

`````js
{}
`````
## Input

`````js
if (a) b;
else let {x};
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 164,
            "ifKeyword": {
                "kind": 37757019,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 2
            },
            "expression": {
                "kind": 134299649,
                "text": "a",
                "rawText": "a",
                "flags": 96,
                "transformFlags": 0,
                "start": 4,
                "end": 5
            },
            "consequent": {
                "kind": 120,
                "expression": {
                    "kind": 134299649,
                    "text": "b",
                    "rawText": "b",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 6,
                    "end": 8
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 6,
                "end": 9
            },
            "elseKeyword": {
                "kind": 4194389,
                "flags": 65,
                "transformFlags": 0,
                "start": 9,
                "end": 14
            },
            "alternate": {
                "kind": 120,
                "expression": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 14,
                    "end": 18
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 14,
                "end": 18
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 18
        },
        {
            "kind": 124,
            "block": {
                "kind": 249,
                "statements": [
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 134299649,
                            "text": "x",
                            "rawText": "x",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 20,
                            "end": 21
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 20,
                        "end": 21
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 20,
                "end": 21
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 18,
            "end": 22
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 22,
            "end": 23
        }
    ],
    "isModule": false,
    "source": "if (a) b;\nelse let {x};",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 23
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ '{' is not allowed here. Did you mean ';'? - start: 18, end: 20

```

