# Kataw parser test case

## Input

`````js
for (let {x = y} = obj);
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
                                "kind": 212,
                                "propertyList": {
                                    "kind": 213,
                                    "properties": [
                                        {
                                            "kind": 281,
                                            "ellipsisToken": null,
                                            "left": {
                                                "kind": 134299649,
                                                "text": "x",
                                                "rawText": "x",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 10,
                                                "end": 11
                                            },
                                            "optionalToken": null,
                                            "type": null,
                                            "right": {
                                                "kind": 134299649,
                                                "text": "y",
                                                "rawText": "y",
                                                "flags": 96,
                                                "transformFlags": 0,
                                                "start": 13,
                                                "end": 15
                                            },
                                            "flags": 0,
                                            "transformFlags": 4096,
                                            "start": 10,
                                            "end": 15
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 10,
                                    "end": 15
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 8,
                                "end": 16
                            },
                            "type": null,
                            "initializer": {
                                "kind": 134299649,
                                "text": "obj",
                                "rawText": "obj",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 18,
                                "end": 22
                            },
                            "flags": 16,
                            "transformFlags": 4224,
                            "start": 8,
                            "end": 22
                        }
                    ],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 8,
                    "end": 22
                },
                "flags": 33554448,
                "transformFlags": 0,
                "start": 0,
                "end": 22
            },
            "condition": null,
            "incrementor": {
                "kind": 16637,
                "text": "",
                "rawText": "",
                "flags": 64,
                "transformFlags": 0,
                "start": 22,
                "end": 22
            },
            "statement": {
                "kind": 168,
                "flags": 16,
                "transformFlags": 0,
                "start": 23,
                "end": 24
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 24
        }
    ],
    "isModule": false,
    "source": "for (let {x = y} = obj);",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 24
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Lexical declaration expected - start: 22, end: 23
✖ Identifier expected - start: 22, end: 23

```

