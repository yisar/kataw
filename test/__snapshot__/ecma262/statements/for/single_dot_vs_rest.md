# Kataw parser test case

## Input

`````js
for (let [.x] = obj);
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 165,
            "forKeyword": {
                "kind": 37757017,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "initializer": {
                "kind": 162,
                "lexicalKeyword": {
                    "kind": 41951307,
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 0,
                    "end": 8
                },
                "binding": {
                    "kind": 151,
                    "bindingList": [
                        {
                            "kind": 190,
                            "binding": {
                                "kind": 201,
                                "elementList": {
                                    "kind": 324,
                                    "elements": [],
                                    "trailingComma": false,
                                    "flags": 0,
                                    "transformFlags": 0,
                                    "start": 10,
                                    "end": 10
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 8,
                                "end": 10
                            },
                            "type": null,
                            "initializer": null,
                            "flags": 16,
                            "transformFlags": 4224,
                            "start": 8,
                            "end": 10
                        }
                    ],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 8,
                    "end": 10
                },
                "flags": 33554448,
                "transformFlags": 0,
                "start": 0,
                "end": 10
            },
            "condition": {
                "kind": 16637,
                "text": "",
                "rawText": "",
                "flags": 64,
                "transformFlags": 0,
                "start": 12,
                "end": 12
            },
            "incrementor": {
                "kind": 129,
                "member": {
                    "kind": 16637,
                    "text": "",
                    "rawText": "",
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 10,
                    "end": 10
                },
                "expression": {
                    "kind": 134299649,
                    "text": "x",
                    "rawText": "x",
                    "flags": 96,
                    "transformFlags": 0,
                    "start": 11,
                    "end": 12
                },
                "flags": 96,
                "transformFlags": 2,
                "start": 10,
                "end": 12
            },
            "statement": {
                "kind": 120,
                "expression": {
                    "kind": 16637,
                    "text": "",
                    "rawText": "",
                    "flags": 64,
                    "transformFlags": 0,
                    "start": 12,
                    "end": 12
                },
                "flags": 16,
                "transformFlags": 4096,
                "start": 12,
                "end": 12
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 12
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "obj",
                "rawText": "obj",
                "flags": 96,
                "transformFlags": 0,
                "start": 15,
                "end": 19
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 15,
            "end": 19
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 20,
            "end": 21
        }
    ],
    "isModule": false,
    "source": "for (let [.x] = obj);",
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
✖ Did you forgot a ']' to match the `[` token? - start: 10, end: 11
✖ Missing initializer in destructuring declaration - start: 10, end: 11
✖ Lexical declaration expected - start: 10, end: 11
✖ Identifier expected - start: 12, end: 13
✖ Declaration or statement expected - start: 13, end: 15
✖ ')' is not allowed here. Did you mean ';'? - start: 19, end: 20

```

