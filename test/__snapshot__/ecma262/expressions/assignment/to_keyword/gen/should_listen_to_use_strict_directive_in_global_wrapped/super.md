# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/assignment/to_keyword/gen/should_listen_to_use_strict_directive_in_global_wrapped
> :: test: should listen to use strict directive in global wrapped
> :: case: super
## Options

`````js
{}
`````
## Input

`````js
"use strict"; (super = x);
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [
        {
            "kind": 201392131,
            "text": "use strict",
            "rawText": "\"use strict\"",
            "flags": 96,
            "transformFlags": 0,
            "start": 0,
            "end": 12
        }
    ],
    "statements": [
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 125,
                    "left": {
                        "kind": 129,
                        "member": {
                            "kind": 4259935,
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 15,
                            "end": 20
                        },
                        "expression": {
                            "kind": 16637,
                            "text": "",
                            "rawText": "",
                            "flags": 64,
                            "transformFlags": 0,
                            "start": 20,
                            "end": 20
                        },
                        "flags": 32,
                        "transformFlags": 2,
                        "start": 15,
                        "end": 20
                    },
                    "operatorToken": {
                        "kind": 4125,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 20,
                        "end": 22
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "x",
                        "rawText": "x",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 22,
                        "end": 24
                    },
                    "flags": 0,
                    "transformFlags": 128,
                    "start": 15,
                    "end": 24
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 13,
                "end": 25
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 13,
            "end": 26
        }
    ],
    "isModule": false,
    "source": "\"use strict\"; (super = x);",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 26
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ 'super' must be followed by an argument list or member access. - start: 15, end: 22
✖ Dot property must be an identifier - start: 20, end: 22
✖ The left-hand side of an assignment expression must be a variable or a property access - start: 20, end: 22

```

