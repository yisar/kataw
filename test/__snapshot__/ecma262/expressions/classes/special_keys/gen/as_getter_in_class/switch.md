# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/classes/special_keys/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/classes/special_keys/gen/as_getter_in_class
> :: test: as getter in class
> :: case: switch
## Options

`````js
{}
`````
## Input

`````js
class x {get switch(){}}
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
            "declareKeyword": null,
            "decorators": null,
            "classKeyword": {
                "kind": 37822544,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 5
            },
            "name": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 5,
                "end": 7
            },
            "typeParameters": null,
            "tail": {
                "kind": 277,
                "classHeritage": null,
                "body": {
                    "kind": 303,
                    "elements": [
                        {
                            "kind": 278,
                            "declareToken": null,
                            "decorators": null,
                            "staticKeyword": null,
                            "asyncKeyword": null,
                            "setKeyword": {
                                "kind": 16498,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 9,
                                "end": 12
                            },
                            "getKeyword": null,
                            "asteriskToken": null,
                            "method": {
                                "kind": 209,
                                "name": {
                                    "kind": 134299649,
                                    "text": "switch",
                                    "rawText": "switch",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 12,
                                    "end": 19
                                },
                                "typeParameters": null,
                                "formalParameterList": {
                                    "kind": 214,
                                    "formalParameters": [],
                                    "trailingComma": false,
                                    "flags": 1024,
                                    "transformFlags": 0,
                                    "start": 20,
                                    "end": 21
                                },
                                "returnType": null,
                                "contents": {
                                    "kind": 216,
                                    "functionStatementList": {
                                        "kind": 217,
                                        "directives": [],
                                        "statements": [],
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 22,
                                        "end": 22
                                    },
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 21,
                                    "end": 23
                                },
                                "flags": 1024,
                                "transformFlags": 0,
                                "start": 19,
                                "end": 23
                            },
                            "flags": 1024,
                            "transformFlags": 0,
                            "start": 9,
                            "end": 23
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 9,
                    "end": 23
                },
                "flags": 7,
                "transformFlags": 0,
                "start": 32,
                "end": 24
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 24
        }
    ],
    "isModule": false,
    "source": "class x {get switch(){}}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 24
}
```

### Printed

```javascript
class x {
  get switch() {}
}
```

### Diagnostics

```javascript
✔ No errors
```

