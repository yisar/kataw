# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/gen/assignment_paren_wrapped
> :: test: assignment paren wrapped
> :: case: \u0065xport
## Options

`````js
{}
`````
## Input

`````js
(\u0065xport = x);
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
                    "kind": 16637,
                    "text": "",
                    "rawText": "",
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 1,
                    "end": 1
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 0,
                "end": 1
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 1
        },
        {
            "kind": 257,
            "exportKeyword": {
                "kind": 4202582,
                "flags": 16464,
                "transformFlags": 0,
                "start": 1,
                "end": 12
            },
            "declaration": null,
            "namedExports": null,
            "exportFromClause": null,
            "fromClause": null,
            "exportKind": 0,
            "flags": 80,
            "transformFlags": 0,
            "start": 1,
            "end": 12
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 14,
                "end": 16
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 14,
            "end": 16
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 17,
            "end": 18
        }
    ],
    "isModule": false,
    "source": "(\\u0065xport = x);",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 18
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Identifier expected - start: 1, end: 12
✖ The `export` keyword can only be used with the module goal - start: 1, end: 12
✖ Keywords cannot contain escape characters - start: 1, end: 12
✖ Declaration or statement expected - start: 12, end: 14
✖ Declaration or statement expected - start: 12, end: 14
✖ ')' is not allowed here. Did you mean ';'? - start: 16, end: 17

```

