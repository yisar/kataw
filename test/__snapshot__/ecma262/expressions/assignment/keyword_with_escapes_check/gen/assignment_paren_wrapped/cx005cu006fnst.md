# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/keyword_with_escapes_check/gen/assignment_paren_wrapped
> :: test: assignment paren wrapped
> :: case: c\u006fnst
## Options

`````js
{}
`````
## Input

`````js
(c\u006fnst = x);
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
            "kind": 162,
            "lexicalKeyword": {
                "kind": 37757004,
                "flags": 16464,
                "transformFlags": 0,
                "start": 1,
                "end": 11
            },
            "binding": {
                "kind": 151,
                "bindingList": [],
                "flags": 16777232,
                "transformFlags": 0,
                "start": 11,
                "end": 11
            },
            "flags": 33554448,
            "transformFlags": 0,
            "start": 1,
            "end": 11
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 13,
                "end": 15
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 13,
            "end": 15
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 16,
            "end": 17
        }
    ],
    "isModule": false,
    "source": "(c\\u006fnst = x);",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 17
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Identifier expected - start: 1, end: 11
✖ Keywords cannot contain escape characters - start: 1, end: 11
✖ '=' is not allowed here. Did you mean ';'? - start: 11, end: 13
✖ ')' is not allowed here. Did you mean ';'? - start: 15, end: 16

```

