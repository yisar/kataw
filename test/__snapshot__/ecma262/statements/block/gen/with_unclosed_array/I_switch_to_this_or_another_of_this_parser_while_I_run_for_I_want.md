# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/statements/block/autogen.md
- Path: kataw/test/__snapshot__/ecma262/statements/block/gen/with_unclosed_array
> :: test: with unclosed array
> :: case: I switch to this or another of this parser while I run for I want
## Options

`````js
{}
`````
## Input

`````js
{[ I switch to this or another of this parser while I run for I want
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
                            "kind": 119,
                            "elementList": {
                                "kind": 270,
                                "elements": [
                                    {
                                        "kind": 134299649,
                                        "text": "I",
                                        "rawText": "I",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 2,
                                        "end": 4
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 2,
                                "end": 4
                            },
                            "flags": 32,
                            "transformFlags": 8,
                            "start": 1,
                            "end": 4
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 1,
                        "end": 4
                    },
                    {
                        "kind": 160,
                        "switchKeyword": {
                            "kind": 37757024,
                            "flags": 80,
                            "transformFlags": 0,
                            "start": 4,
                            "end": 11
                        },
                        "expression": {
                            "kind": 134299649,
                            "text": "to",
                            "rawText": "to",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 11,
                            "end": 14
                        },
                        "caseBlock": {
                            "kind": 152,
                            "clauses": [],
                            "flags": 16,
                            "transformFlags": 0,
                            "start": 14,
                            "end": 14
                        },
                        "flags": 80,
                        "transformFlags": 0,
                        "start": 4,
                        "end": 14
                    },
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 4276321,
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 14,
                            "end": 19
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 14,
                        "end": 19
                    },
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 134299649,
                            "text": "or",
                            "rawText": "or",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 19,
                            "end": 22
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 19,
                        "end": 22
                    },
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 134299649,
                            "text": "another",
                            "rawText": "another",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 22,
                            "end": 30
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 22,
                        "end": 30
                    },
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 134299649,
                            "text": "of",
                            "rawText": "of",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 30,
                            "end": 33
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 30,
                        "end": 33
                    },
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 4276321,
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 33,
                            "end": 38
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 33,
                        "end": 38
                    },
                    {
                        "kind": 120,
                        "expression": {
                            "kind": 134299649,
                            "text": "parser",
                            "rawText": "parser",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 38,
                            "end": 45
                        },
                        "flags": 16,
                        "transformFlags": 4096,
                        "start": 38,
                        "end": 45
                    },
                    {
                        "kind": 154,
                        "whileKeyword": {
                            "kind": 37757028,
                            "flags": 80,
                            "transformFlags": 0,
                            "start": 45,
                            "end": 51
                        },
                        "expression": {
                            "kind": 134299649,
                            "text": "I",
                            "rawText": "I",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 51,
                            "end": 53
                        },
                        "statement": {
                            "kind": 120,
                            "expression": {
                                "kind": 134299649,
                                "text": "run",
                                "rawText": "run",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 53,
                                "end": 57
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 53,
                            "end": 57
                        },
                        "flags": 80,
                        "transformFlags": 0,
                        "start": 45,
                        "end": 57
                    },
                    {
                        "kind": 165,
                        "forKeyword": {
                            "kind": 37757017,
                            "flags": 80,
                            "transformFlags": 0,
                            "start": 57,
                            "end": 61
                        },
                        "initializer": {
                            "kind": 134299649,
                            "text": "I",
                            "rawText": "I",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 61,
                            "end": 63
                        },
                        "condition": {
                            "kind": 16637,
                            "text": "",
                            "rawText": "",
                            "flags": 64,
                            "transformFlags": 0,
                            "start": 68,
                            "end": 68
                        },
                        "incrementor": {
                            "kind": 134299649,
                            "text": "want",
                            "rawText": "want",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 63,
                            "end": 68
                        },
                        "statement": {
                            "kind": 120,
                            "expression": {
                                "kind": 16637,
                                "text": "",
                                "rawText": "",
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 68,
                                "end": 68
                            },
                            "flags": 16,
                            "transformFlags": 4096,
                            "start": 68,
                            "end": 68
                        },
                        "flags": 80,
                        "transformFlags": 0,
                        "start": 57,
                        "end": 68
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 1,
                "end": 68
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 68
        }
    ],
    "isModule": false,
    "source": "{[ I switch to this or another of this parser while I run for I want",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 68
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ ',' expected - start: 5, end: 11
✖ Missing an opening parentheses - '( - start: 12, end: 14
✖ Declaration or statement expected - start: 15, end: 19
✖ '; ' is not allowed here. Did you mean ';'? - start: 19, end: 22
✖ '; ' is not allowed here. Did you mean ';'? - start: 22, end: 30
✖ 'of' is not allowed here. Did you mean ';'? - start: 30, end: 33
✖ 'this' is not allowed here. Did you mean ';'? - start: 33, end: 38
✖ '; ' is not allowed here. Did you mean ';'? - start: 38, end: 45
✖ 'while' is not allowed here. Did you mean ';'? - start: 45, end: 51
✖ Missing an opening parentheses - '( - start: 52, end: 53
✖ Declaration or statement expected - start: 54, end: 57
✖ 'for' is not allowed here. Did you mean ';'? - start: 57, end: 61
✖ Missing an opening parentheses - '( - start: 62, end: 63
✖ Identifier expected - start: 68, end: 68

```

