# Kataw parser test case

## Input

`````js
for (let [foo] = arr, [bar] = arr2);
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
                                    "elements": [
                                        {
                                            "kind": 134299649,
                                            "text": "foo",
                                            "rawText": "foo",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 10,
                                            "end": 13
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 0,
                                    "transformFlags": 0,
                                    "start": 10,
                                    "end": 13
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 8,
                                "end": 14
                            },
                            "type": null,
                            "initializer": {
                                "kind": 134299649,
                                "text": "arr",
                                "rawText": "arr",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 16,
                                "end": 20
                            },
                            "flags": 16,
                            "transformFlags": 4224,
                            "start": 8,
                            "end": 20
                        },
                        {
                            "kind": 190,
                            "binding": {
                                "kind": 201,
                                "elementList": {
                                    "kind": 324,
                                    "elements": [
                                        {
                                            "kind": 134299649,
                                            "text": "bar",
                                            "rawText": "bar",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 23,
                                            "end": 26
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 0,
                                    "transformFlags": 0,
                                    "start": 23,
                                    "end": 26
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 21,
                                "end": 27
                            },
                            "type": null,
                            "initializer": {
                                "kind": 134299649,
                                "text": "arr2",
                                "rawText": "arr2",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 29,
                                "end": 34
                            },
                            "flags": 16,
                            "transformFlags": 4224,
                            "start": 21,
                            "end": 34
                        }
                    ],
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 8,
                    "end": 34
                },
                "flags": 33554448,
                "transformFlags": 0,
                "start": 0,
                "end": 34
            },
            "condition": null,
            "incrementor": {
                "kind": 16637,
                "text": "",
                "rawText": "",
                "flags": 64,
                "transformFlags": 0,
                "start": 34,
                "end": 34
            },
            "statement": {
                "kind": 168,
                "flags": 16,
                "transformFlags": 0,
                "start": 35,
                "end": 36
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 36
        }
    ],
    "isModule": false,
    "source": "for (let [foo] = arr, [bar] = arr2);",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 36
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Lexical declaration expected - start: 34, end: 35
✖ Identifier expected - start: 34, end: 35

```

