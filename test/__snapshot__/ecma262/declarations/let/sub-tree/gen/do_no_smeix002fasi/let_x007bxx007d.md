# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/declarations/let/sub-tree/autogen.md
- Path: kataw/test/__snapshot__/ecma262/declarations/let/sub-tree/gen/do_no_smeix002fasi
> :: test: do no smei/asi
> :: case: let {x}
## Options

`````js
{}
`````
## Input

`````js
do let {x} while (a);
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 169,
            "doKeyword": {
                "kind": 4202580,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 2
            },
            "statement": {
                "kind": 120,
                "expression": {
                    "kind": 134299649,
                    "text": "let",
                    "rawText": "let",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 2,
                    "end": 6
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 2,
                "end": 6
            },
            "whileKeyword": null,
            "expression": {
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
                            "start": 8,
                            "end": 9
                        }
                    ],
                    "trailingComma": false,
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 8,
                    "end": 9
                },
                "flags": 48,
                "transformFlags": 8,
                "start": 6,
                "end": 10
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 10
        },
        {
            "kind": 154,
            "whileKeyword": {
                "kind": 37757028,
                "flags": 80,
                "transformFlags": 0,
                "start": 10,
                "end": 16
            },
            "expression": {
                "kind": 134299649,
                "text": "a",
                "rawText": "a",
                "flags": 96,
                "transformFlags": 0,
                "start": 18,
                "end": 19
            },
            "statement": {
                "kind": 168,
                "flags": 16,
                "transformFlags": 0,
                "start": 20,
                "end": 21
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 10,
            "end": 21
        }
    ],
    "isModule": false,
    "source": "do let {x} while (a);",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 21
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ '{' is not allowed here. Did you mean ';'? - start: 6, end: 8
✖ Declaration or statement expected - start: 11, end: 16

```

