# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/super/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/super/gen/obj-expr-method-gen
> :: test: obj-expr-method-gen
> :: case: var f = function { super(); }
## Options

`````js
{}
`````
## Input

`````js
({ *method() { var f = function { super(); } } })
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
                    "kind": 132,
                    "expressions": [],
                    "flags": 32,
                    "transformFlags": 1024,
                    "start": 0,
                    "end": 46
                },
                "flags": 34,
                "transformFlags": 0,
                "start": 0,
                "end": 46
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 46
        }
    ],
    "isModule": false,
    "source": "({ *method() { var f = function { super(); } } })",
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
✖ Missing an opening parentheses - '( - start: 32, end: 33
✖ Object literal keys that are strings or numbers must be a method or have a colon - start: 39, end: 40
✖ ',' expected - start: 39, end: 40
✖ Expected a ')' to match the '(' token here - start: 47, end: 48
✖ Declaration or statement expected - start: 48, end: 49

```

