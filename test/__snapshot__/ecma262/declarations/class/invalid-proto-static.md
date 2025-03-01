# Kataw parser test case

## Input

`````js
declare class C {
  proto static p: T;
}
`````

## Options

### Parser Options

`````js
{ allowTypes : true }
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 178,
            "declareKeyword": {
                "kind": 82165,
                "flags": 64,
                "transformFlags": 0,
                "start": 0,
                "end": 7
            },
            "decorators": null,
            "classKeyword": {
                "kind": 37822544,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 13
            },
            "name": {
                "kind": 134299649,
                "text": "C",
                "rawText": "C",
                "flags": 96,
                "transformFlags": 0,
                "start": 13,
                "end": 15
            },
            "typeParameters": null,
            "tail": {
                "kind": 277,
                "classHeritage": null,
                "body": {
                    "kind": 134234353,
                    "properties": [
                        {
                            "kind": 193,
                            "protoKeyword": {
                                "kind": 16873,
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 17,
                                "end": 25
                            },
                            "staticKeyword": null,
                            "getKeyword": null,
                            "setKeyword": null,
                            "key": {
                                "kind": 134299649,
                                "text": "static",
                                "rawText": "static",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 25,
                                "end": 32
                            },
                            "optionalToken": null,
                            "type": {
                                "kind": 139,
                                "bitwiseOrToken": null,
                                "bitwiseAndToken": null,
                                "type": {
                                    "kind": 144,
                                    "typeName": {
                                        "kind": 134299649,
                                        "text": "p",
                                        "rawText": "p",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 32,
                                        "end": 34
                                    },
                                    "typeParameters": null,
                                    "flags": 2097152,
                                    "transformFlags": 0,
                                    "start": 32,
                                    "end": 34
                                },
                                "flags": 2097152,
                                "transformFlags": 0,
                                "start": 32,
                                "end": 34
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 17,
                            "end": 34
                        }
                    ],
                    "trailingComma": false,
                    "flags": 2097152,
                    "transformFlags": 0,
                    "start": 15,
                    "end": 34
                },
                "flags": 4128,
                "transformFlags": 0,
                "start": 15,
                "end": 34
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 34
        },
        {
            "kind": 120,
            "expression": {
                "kind": 134299649,
                "text": "T",
                "rawText": "T",
                "flags": 96,
                "transformFlags": 0,
                "start": 35,
                "end": 37
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 35,
            "end": 38
        }
    ],
    "isModule": false,
    "source": "declare class C {\n  proto static p: T;\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 40
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ ':' is not allowed here. Did you mean ';'? - start: 34, end: 35
✖ Declaration or statement expected - start: 38, end: 40

```

