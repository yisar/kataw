# Kataw parser test case

## Input

`````js
this.foo[foo].bar(this)(bar)[foo]()--
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
                "kind": 127,
                "operandToken": {
                    "kind": 196636,
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 35,
                    "end": 37
                },
                "operand": {
                    "kind": 131,
                    "expression": {
                        "kind": 130,
                        "member": {
                            "kind": 131,
                            "expression": {
                                "kind": 131,
                                "expression": {
                                    "kind": 129,
                                    "member": {
                                        "kind": 130,
                                        "member": {
                                            "kind": 129,
                                            "member": {
                                                "kind": 4276321,
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 0,
                                                "end": 4
                                            },
                                            "expression": {
                                                "kind": 134299649,
                                                "text": "foo",
                                                "rawText": "foo",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 5,
                                                "end": 8
                                            },
                                            "flags": 96,
                                            "transformFlags": 2,
                                            "start": 0,
                                            "end": 8
                                        },
                                        "expression": {
                                            "kind": 134299649,
                                            "text": "foo",
                                            "rawText": "foo",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 9,
                                            "end": 12
                                        },
                                        "flags": 32,
                                        "transformFlags": 4,
                                        "start": 0,
                                        "end": 13
                                    },
                                    "expression": {
                                        "kind": 134299649,
                                        "text": "bar",
                                        "rawText": "bar",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 14,
                                        "end": 17
                                    },
                                    "flags": 32,
                                    "transformFlags": 2,
                                    "start": 0,
                                    "end": 17
                                },
                                "argumentList": {
                                    "kind": 256,
                                    "elements": [
                                        {
                                            "kind": 4276321,
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 18,
                                            "end": 22
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 18,
                                    "end": 22
                                },
                                "flags": 32,
                                "transformFlags": 1,
                                "start": 0,
                                "end": 23
                            },
                            "argumentList": {
                                "kind": 256,
                                "elements": [
                                    {
                                        "kind": 134299649,
                                        "text": "bar",
                                        "rawText": "bar",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 24,
                                        "end": 27
                                    }
                                ],
                                "trailingComma": false,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 24,
                                "end": 27
                            },
                            "flags": 32,
                            "transformFlags": 1,
                            "start": 0,
                            "end": 28
                        },
                        "expression": {
                            "kind": 134299649,
                            "text": "foo",
                            "rawText": "foo",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 29,
                            "end": 32
                        },
                        "flags": 32,
                        "transformFlags": 4,
                        "start": 0,
                        "end": 33
                    },
                    "argumentList": {
                        "kind": 256,
                        "elements": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 34,
                        "end": 34
                    },
                    "flags": 32,
                    "transformFlags": 1,
                    "start": 0,
                    "end": 35
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 0,
                "end": 37
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 37
        }
    ],
    "isModule": false,
    "source": "this.foo[foo].bar(this)(bar)[foo]()--",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 37
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ The operand of an increment or decrement operator must be a variable or a property access - start: 35, end: 37

```

