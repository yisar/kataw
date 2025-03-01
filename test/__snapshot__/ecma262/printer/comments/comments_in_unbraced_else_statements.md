# Kataw parser test case

## Input

`````js
if (firstTrue())
  // comment
  doFirstThing();
else if (secondTrue())
  // comment
  doSecondThing();
else
  // this comment should not move
  doThirdThing()
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
                "kind": 131,
                "expression": {
                    "kind": 134299649,
                    "text": "firstTrue",
                    "rawText": "firstTrue",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 4,
                    "end": 13
                },
                "argumentList": {
                    "kind": 256,
                    "elements": [],
                    "trailingComma": false,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 14,
                    "end": 14
                },
                "flags": 32,
                "transformFlags": 1,
                "start": 4,
                "end": 15
            },
            "consequent": {
                "kind": 120,
                "expression": {
                    "kind": 131,
                    "expression": {
                        "kind": 134299649,
                        "text": "doFirstThing",
                        "rawText": "doFirstThing",
                        "flags": 97,
                        "transformFlags": 0,
                        "start": 16,
                        "end": 44
                    },
                    "argumentList": {
                        "kind": 256,
                        "elements": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 45,
                        "end": 45
                    },
                    "flags": 32,
                    "transformFlags": 1,
                    "start": 16,
                    "end": 46
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 16,
                "end": 47
            },
            "elseKeyword": {
                "kind": 4194389,
                "flags": 65,
                "transformFlags": 0,
                "start": 47,
                "end": 52
            },
            "alternate": {
                "kind": 164,
                "ifKeyword": {
                    "kind": 37757019,
                    "flags": 80,
                    "transformFlags": 0,
                    "start": 52,
                    "end": 55
                },
                "expression": {
                    "kind": 131,
                    "expression": {
                        "kind": 134299649,
                        "text": "secondTrue",
                        "rawText": "secondTrue",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 57,
                        "end": 67
                    },
                    "argumentList": {
                        "kind": 256,
                        "elements": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 68,
                        "end": 68
                    },
                    "flags": 32,
                    "transformFlags": 1,
                    "start": 57,
                    "end": 69
                },
                "consequent": {
                    "kind": 120,
                    "expression": {
                        "kind": 131,
                        "expression": {
                            "kind": 134299649,
                            "text": "doSecondThing",
                            "rawText": "doSecondThing",
                            "flags": 97,
                            "transformFlags": 0,
                            "start": 70,
                            "end": 99
                        },
                        "argumentList": {
                            "kind": 256,
                            "elements": [],
                            "trailingComma": false,
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 100,
                            "end": 100
                        },
                        "flags": 32,
                        "transformFlags": 1,
                        "start": 70,
                        "end": 101
                    },
                    "flags": 16,
                    "transformFlags": 4096,
                    "start": 70,
                    "end": 102
                },
                "elseKeyword": {
                    "kind": 4194389,
                    "flags": 65,
                    "transformFlags": 0,
                    "start": 102,
                    "end": 107
                },
                "alternate": {
                    "kind": 120,
                    "expression": {
                        "kind": 131,
                        "expression": {
                            "kind": 134299649,
                            "text": "doThirdThing",
                            "rawText": "doThirdThing",
                            "flags": 97,
                            "transformFlags": 0,
                            "start": 107,
                            "end": 156
                        },
                        "argumentList": {
                            "kind": 256,
                            "elements": [],
                            "trailingComma": false,
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 157,
                            "end": 157
                        },
                        "flags": 32,
                        "transformFlags": 1,
                        "start": 107,
                        "end": 158
                    },
                    "flags": 16,
                    "transformFlags": 4096,
                    "start": 107,
                    "end": 158
                },
                "flags": 80,
                "transformFlags": 0,
                "start": 52,
                "end": 158
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 158
        }
    ],
    "isModule": false,
    "source": "if (firstTrue())\n  // comment\n  doFirstThing();\nelse if (secondTrue())\n  // comment\n  doSecondThing();\nelse\n  // this comment should not move\n  doThirdThing()",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 158
}
```

### Printed

```javascript
if (firstTrue()) // comment
  doFirstThing();
else  if (secondTrue()) // comment
  doSecondThing();
else  // this comment should not move
  doThirdThing();
```

### Diagnostics

```javascript
✔ No errors
```

