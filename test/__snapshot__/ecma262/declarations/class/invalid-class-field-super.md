# Kataw parser test case

## Input

`````js
class C { aaa = super.bbb };

class C { aaa = () => super.bbb };

class C { aaa = () => () => super.bbb };

class C { [super.bbb] = 0 };

`````

## Options

### Parser Options

`````js
{}
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
                "text": "C",
                "rawText": "C",
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
                            "kind": 280,
                            "decorators": null,
                            "declaredToken": null,
                            "staticKeyword": null,
                            "asyncKeyword": null,
                            "key": {
                                "kind": 134299649,
                                "text": "aaa",
                                "rawText": "aaa",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 9,
                                "end": 13
                            },
                            "optionalToken": null,
                            "type": null,
                            "initializer": {
                                "kind": 129,
                                "member": {
                                    "kind": 4259935,
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 15,
                                    "end": 21
                                },
                                "expression": {
                                    "kind": 134299649,
                                    "text": "bbb",
                                    "rawText": "bbb",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 22,
                                    "end": 25
                                },
                                "flags": 96,
                                "transformFlags": 2,
                                "start": 15,
                                "end": 25
                            },
                            "flags": 32,
                            "transformFlags": 128,
                            "start": 9,
                            "end": 25
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 9,
                    "end": 25
                },
                "flags": 7,
                "transformFlags": 0,
                "start": 32,
                "end": 27
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 27
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 27,
            "end": 28
        },
        {
            "kind": 178,
            "declareKeyword": null,
            "decorators": null,
            "classKeyword": {
                "kind": 37822544,
                "flags": 81,
                "transformFlags": 0,
                "start": 28,
                "end": 35
            },
            "name": {
                "kind": 134299649,
                "text": "C",
                "rawText": "C",
                "flags": 96,
                "transformFlags": 0,
                "start": 35,
                "end": 37
            },
            "typeParameters": null,
            "tail": {
                "kind": 277,
                "classHeritage": null,
                "body": {
                    "kind": 303,
                    "elements": [
                        {
                            "kind": 280,
                            "decorators": null,
                            "declaredToken": null,
                            "staticKeyword": null,
                            "asyncKeyword": null,
                            "key": {
                                "kind": 134299649,
                                "text": "aaa",
                                "rawText": "aaa",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 39,
                                "end": 43
                            },
                            "optionalToken": null,
                            "type": null,
                            "initializer": {
                                "kind": 271,
                                "asyncKeyword": null,
                                "typeParameters": null,
                                "arrowPatameterList": {
                                    "kind": 342,
                                    "parameters": [],
                                    "trailingComma": false,
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 47,
                                    "end": 47
                                },
                                "returnType": null,
                                "arrowToken": {
                                    "kind": 10,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 48,
                                    "end": 51
                                },
                                "contents": {
                                    "kind": 129,
                                    "member": {
                                        "kind": 4259935,
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 51,
                                        "end": 57
                                    },
                                    "expression": {
                                        "kind": 134299649,
                                        "text": "bbb",
                                        "rawText": "bbb",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 58,
                                        "end": 61
                                    },
                                    "flags": 96,
                                    "transformFlags": 2,
                                    "start": 51,
                                    "end": 61
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 45,
                                "end": 61
                            },
                            "flags": 32,
                            "transformFlags": 128,
                            "start": 39,
                            "end": 61
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 39,
                    "end": 61
                },
                "flags": 37,
                "transformFlags": 0,
                "start": 32,
                "end": 63
            },
            "flags": 17,
            "transformFlags": 0,
            "start": 28,
            "end": 63
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 63,
            "end": 64
        },
        {
            "kind": 178,
            "declareKeyword": null,
            "decorators": null,
            "classKeyword": {
                "kind": 37822544,
                "flags": 81,
                "transformFlags": 0,
                "start": 64,
                "end": 71
            },
            "name": {
                "kind": 134299649,
                "text": "C",
                "rawText": "C",
                "flags": 96,
                "transformFlags": 0,
                "start": 71,
                "end": 73
            },
            "typeParameters": null,
            "tail": {
                "kind": 277,
                "classHeritage": null,
                "body": {
                    "kind": 303,
                    "elements": [
                        {
                            "kind": 280,
                            "decorators": null,
                            "declaredToken": null,
                            "staticKeyword": null,
                            "asyncKeyword": null,
                            "key": {
                                "kind": 134299649,
                                "text": "aaa",
                                "rawText": "aaa",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 75,
                                "end": 79
                            },
                            "optionalToken": null,
                            "type": null,
                            "initializer": {
                                "kind": 271,
                                "asyncKeyword": null,
                                "typeParameters": null,
                                "arrowPatameterList": {
                                    "kind": 342,
                                    "parameters": [],
                                    "trailingComma": false,
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 83,
                                    "end": 83
                                },
                                "returnType": null,
                                "arrowToken": {
                                    "kind": 10,
                                    "flags": 64,
                                    "transformFlags": 0,
                                    "start": 84,
                                    "end": 87
                                },
                                "contents": {
                                    "kind": 271,
                                    "asyncKeyword": null,
                                    "typeParameters": null,
                                    "arrowPatameterList": {
                                        "kind": 342,
                                        "parameters": [],
                                        "trailingComma": false,
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 89,
                                        "end": 89
                                    },
                                    "returnType": null,
                                    "arrowToken": {
                                        "kind": 10,
                                        "flags": 64,
                                        "transformFlags": 0,
                                        "start": 90,
                                        "end": 93
                                    },
                                    "contents": {
                                        "kind": 129,
                                        "member": {
                                            "kind": 4259935,
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 93,
                                            "end": 99
                                        },
                                        "expression": {
                                            "kind": 134299649,
                                            "text": "bbb",
                                            "rawText": "bbb",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 100,
                                            "end": 103
                                        },
                                        "flags": 96,
                                        "transformFlags": 2,
                                        "start": 93,
                                        "end": 103
                                    },
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 87,
                                    "end": 103
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 81,
                                "end": 103
                            },
                            "flags": 32,
                            "transformFlags": 128,
                            "start": 75,
                            "end": 103
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 75,
                    "end": 103
                },
                "flags": 73,
                "transformFlags": 0,
                "start": 32,
                "end": 105
            },
            "flags": 17,
            "transformFlags": 0,
            "start": 64,
            "end": 105
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 105,
            "end": 106
        },
        {
            "kind": 178,
            "declareKeyword": null,
            "decorators": null,
            "classKeyword": {
                "kind": 37822544,
                "flags": 81,
                "transformFlags": 0,
                "start": 106,
                "end": 113
            },
            "name": {
                "kind": 134299649,
                "text": "C",
                "rawText": "C",
                "flags": 96,
                "transformFlags": 0,
                "start": 113,
                "end": 115
            },
            "typeParameters": null,
            "tail": {
                "kind": 277,
                "classHeritage": null,
                "body": {
                    "kind": 303,
                    "elements": [
                        {
                            "kind": 280,
                            "decorators": null,
                            "declaredToken": null,
                            "staticKeyword": null,
                            "asyncKeyword": null,
                            "key": {
                                "kind": 194,
                                "expression": {
                                    "kind": 129,
                                    "member": {
                                        "kind": 4259935,
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 119,
                                        "end": 124
                                    },
                                    "expression": {
                                        "kind": 134299649,
                                        "text": "bbb",
                                        "rawText": "bbb",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 125,
                                        "end": 128
                                    },
                                    "flags": 96,
                                    "transformFlags": 2,
                                    "start": 119,
                                    "end": 128
                                },
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 117,
                                "end": 129
                            },
                            "optionalToken": null,
                            "type": null,
                            "initializer": {
                                "kind": 201392130,
                                "text": 0,
                                "rawText": "0",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 131,
                                "end": 133
                            },
                            "flags": 32,
                            "transformFlags": 128,
                            "start": 117,
                            "end": 133
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 117,
                    "end": 133
                },
                "flags": 115,
                "transformFlags": 0,
                "start": 32,
                "end": 135
            },
            "flags": 17,
            "transformFlags": 0,
            "start": 106,
            "end": 135
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 135,
            "end": 136
        }
    ],
    "isModule": false,
    "source": "class C { aaa = super.bbb };\n\nclass C { aaa = () => super.bbb };\n\nclass C { aaa = () => () => super.bbb };\n\nclass C { [super.bbb] = 0 };\n",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 137
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ 'super' can only be referenced in members of derived classes or object literal expressions - start: 15, end: 22
✖ Duplicate bindingidentifier 'C' - start: 35, end: 37
✖ 'super' can only be referenced in members of derived classes or object literal expressions - start: 51, end: 58
✖ Duplicate bindingidentifier 'C' - start: 71, end: 73
✖ 'super' can only be referenced in members of derived classes or object literal expressions - start: 93, end: 100
✖ Duplicate bindingidentifier 'C' - start: 113, end: 115
✖ 'super' can only be referenced in members of derived classes or object literal expressions - start: 119, end: 125

```

