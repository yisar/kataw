# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/declarations/let/binding-pattern/autogen.md
- Path: kataw/test/__snapshot__/ecma262/declarations/let/binding-pattern/gen/shorthand_that_is_a_member_expression
> :: test: shorthand that is a member expression
> :: case: let
## Options

`````js
{}
`````
## Input

`````js
let {a.b} = v
`````
## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 162,
            "lexicalKeyword": {
                "kind": 41951307,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "binding": {
                "kind": 151,
                "bindingList": [
                    {
                        "kind": 190,
                        "binding": {
                            "kind": 212,
                            "propertyList": {
                                "kind": 213,
                                "properties": [
                                    {
                                        "kind": 134299649,
                                        "text": "a",
                                        "rawText": "a",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 5,
                                        "end": 6
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 5,
                                "end": 6
                            },
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 6
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 3,
                        "end": 6
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 6
            },
            "flags": 33554448,
            "transformFlags": 0,
            "start": 0,
            "end": 6
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "b",
                "rawText": "b",
                "flags": 96,
                "transformFlags": 0,
                "start": 7,
                "end": 8
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 7,
            "end": 8
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "v",
                "rawText": "v",
                "flags": 96,
                "transformFlags": 0,
                "start": 11,
                "end": 13
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 11,
            "end": 13
        }
    ],
    "isModule": false,
    "source": "let {a.b} = v",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 13
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ ',' expected - start: 6, end: 7
✖ The parser expected to find a '}' to match the '{' token here - start: 6, end: 7
✖ Missing initializer in destructuring declaration - start: 6, end: 7
✖ Lexical declaration expected - start: 6, end: 7
✖ Declaration or statement expected - start: 8, end: 9
✖ Declaration or statement expected - start: 9, end: 11

```

