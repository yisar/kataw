# Kataw parser test case

## Input

`````js
class x extends y { constructor(){ return async function(a=super[foo]) {}; }}
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
                "classHeritage": {
                    "kind": 279,
                    "extendsKeyword": {
                        "kind": 4194391,
                        "flags": 80,
                        "transformFlags": 0,
                        "start": 7,
                        "end": 15
                    },
                    "expression": {
                        "kind": 134299649,
                        "text": "y",
                        "rawText": "y",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 15,
                        "end": 17
                    },
                    "typeParameter": null,
                    "flags": 16,
                    "transformFlags": 0,
                    "start": 15,
                    "end": 17
                },
                "body": {
                    "kind": 303,
                    "elements": [
                        {
                            "kind": 278,
                            "declareToken": null,
                            "decorators": null,
                            "staticKeyword": null,
                            "asyncKeyword": null,
                            "setKeyword": null,
                            "getKeyword": null,
                            "asteriskToken": null,
                            "method": {
                                "kind": 209,
                                "name": {
                                    "kind": 134299649,
                                    "text": "constructor",
                                    "rawText": "constructor",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 19,
                                    "end": 31
                                },
                                "typeParameters": null,
                                "formalParameterList": {
                                    "kind": 214,
                                    "formalParameters": [],
                                    "trailingComma": false,
                                    "flags": 2048,
                                    "transformFlags": 0,
                                    "start": 32,
                                    "end": 33
                                },
                                "returnType": null,
                                "contents": {
                                    "kind": 216,
                                    "functionStatementList": {
                                        "kind": 217,
                                        "directives": [],
                                        "statements": [
                                            {
                                                "kind": 161,
                                                "returnKeyword": {
                                                    "kind": 37757022,
                                                    "flags": 80,
                                                    "transformFlags": 0,
                                                    "start": 34,
                                                    "end": 41
                                                },
                                                "expression": {
                                                    "kind": 177,
                                                    "asyncKeyword": {
                                                        "kind": 82031,
                                                        "flags": 64,
                                                        "transformFlags": 0,
                                                        "start": 41,
                                                        "end": 47
                                                    },
                                                    "functionKeyword": {
                                                        "kind": 37822554,
                                                        "flags": 64,
                                                        "transformFlags": 0,
                                                        "start": 47,
                                                        "end": 56
                                                    },
                                                    "asteriskToken": null,
                                                    "name": null,
                                                    "typeParameters": null,
                                                    "formalParameterList": {
                                                        "kind": 214,
                                                        "formalParameters": [
                                                            {
                                                                "kind": 281,
                                                                "ellipsisToken": null,
                                                                "left": {
                                                                    "kind": 134299649,
                                                                    "text": "a",
                                                                    "rawText": "a",
                                                                    "flags": 96,
                                                                    "transformFlags": 0,
                                                                    "start": 57,
                                                                    "end": 58
                                                                },
                                                                "optionalToken": null,
                                                                "type": null,
                                                                "right": {
                                                                    "kind": 130,
                                                                    "member": {
                                                                        "kind": 4259935,
                                                                        "flags": 96,
                                                                        "transformFlags": 0,
                                                                        "start": 59,
                                                                        "end": 64
                                                                    },
                                                                    "expression": {
                                                                        "kind": 134299649,
                                                                        "text": "foo",
                                                                        "rawText": "foo",
                                                                        "flags": 96,
                                                                        "transformFlags": 0,
                                                                        "start": 65,
                                                                        "end": 68
                                                                    },
                                                                    "flags": 32,
                                                                    "transformFlags": 4,
                                                                    "start": 59,
                                                                    "end": 69
                                                                },
                                                                "flags": 34,
                                                                "transformFlags": 4096,
                                                                "start": 57,
                                                                "end": 69
                                                            }
                                                        ],
                                                        "trailingComma": false,
                                                        "flags": 34,
                                                        "transformFlags": 0,
                                                        "start": 57,
                                                        "end": 69
                                                    },
                                                    "contents": {
                                                        "kind": 216,
                                                        "functionStatementList": {
                                                            "kind": 217,
                                                            "directives": [],
                                                            "statements": [],
                                                            "flags": 32,
                                                            "transformFlags": 0,
                                                            "start": 72,
                                                            "end": 72
                                                        },
                                                        "flags": 32,
                                                        "transformFlags": 0,
                                                        "start": 70,
                                                        "end": 73
                                                    },
                                                    "returnType": null,
                                                    "flags": 160,
                                                    "transformFlags": 0,
                                                    "start": 41,
                                                    "end": 73
                                                },
                                                "flags": 80,
                                                "transformFlags": 256,
                                                "start": 34,
                                                "end": 74
                                            }
                                        ],
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 34,
                                        "end": 74
                                    },
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 33,
                                    "end": 76
                                },
                                "flags": 2048,
                                "transformFlags": 0,
                                "start": 31,
                                "end": 76
                            },
                            "flags": 2048,
                            "transformFlags": 0,
                            "start": 19,
                            "end": 76
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 19,
                    "end": 76
                },
                "flags": 7,
                "transformFlags": 0,
                "start": 32,
                "end": 77
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 77
        }
    ],
    "isModule": false,
    "source": "class x extends y { constructor(){ return async function(a=super[foo]) {}; }}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 77
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ 'super' can only be referenced in members of derived classes or object literal expressions - start: 59, end: 65

```

