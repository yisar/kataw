# Auto-generated test cases ( Kataw )
- From: kataw/test/__snapshot__/ecma262/expressions/super/autogen.md
- Path: kataw/test/__snapshot__/ecma262/expressions/super/gen/class-set
> :: test: class-set
> :: case: var f = function { super(); }
## Options

`````js
{}
`````
## Input

`````js
class C { set x(_) { var f = function { super(); } } }
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
                            "kind": 278,
                            "declareToken": null,
                            "decorators": null,
                            "staticKeyword": null,
                            "asyncKeyword": null,
                            "setKeyword": null,
                            "getKeyword": {
                                "kind": 16499,
                                "flags": 64,
                                "transformFlags": 0,
                                "start": 9,
                                "end": 13
                            },
                            "asteriskToken": null,
                            "method": {
                                "kind": 209,
                                "name": {
                                    "kind": 134299649,
                                    "text": "x",
                                    "rawText": "x",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 13,
                                    "end": 15
                                },
                                "typeParameters": null,
                                "formalParameterList": {
                                    "kind": 214,
                                    "formalParameters": [
                                        {
                                            "kind": 134299649,
                                            "text": "_",
                                            "rawText": "_",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 16,
                                            "end": 17
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 608,
                                    "transformFlags": 0,
                                    "start": 16,
                                    "end": 18
                                },
                                "returnType": null,
                                "contents": {
                                    "kind": 216,
                                    "functionStatementList": {
                                        "kind": 217,
                                        "directives": [],
                                        "statements": [
                                            {
                                                "kind": 155,
                                                "declareKeyword": null,
                                                "varKeyword": {
                                                    "kind": 37757002,
                                                    "flags": 80,
                                                    "transformFlags": 0,
                                                    "start": 20,
                                                    "end": 24
                                                },
                                                "declarationList": {
                                                    "kind": 156,
                                                    "declarations": [
                                                        {
                                                            "kind": 157,
                                                            "binding": {
                                                                "kind": 134299649,
                                                                "text": "f",
                                                                "rawText": "f",
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 24,
                                                                "end": 26
                                                            },
                                                            "type": null,
                                                            "initializer": {
                                                                "kind": 131,
                                                                "expression": {
                                                                    "kind": 177,
                                                                    "asyncKeyword": null,
                                                                    "functionKeyword": {
                                                                        "kind": 37822554,
                                                                        "flags": 64,
                                                                        "transformFlags": 0,
                                                                        "start": 28,
                                                                        "end": 37
                                                                    },
                                                                    "asteriskToken": null,
                                                                    "name": null,
                                                                    "typeParameters": null,
                                                                    "formalParameterList": {
                                                                        "kind": 214,
                                                                        "formalParameters": [
                                                                            {
                                                                                "kind": 212,
                                                                                "propertyList": {
                                                                                    "kind": 213,
                                                                                    "properties": [
                                                                                        {
                                                                                            "kind": 329,
                                                                                            "key": {
                                                                                                "kind": 134299649,
                                                                                                "text": "super",
                                                                                                "rawText": "super",
                                                                                                "flags": 96,
                                                                                                "transformFlags": 0,
                                                                                                "start": 39,
                                                                                                "end": 45
                                                                                            },
                                                                                            "value": {
                                                                                                "kind": 16637,
                                                                                                "text": "",
                                                                                                "rawText": "",
                                                                                                "flags": 64,
                                                                                                "transformFlags": 0,
                                                                                                "start": 45,
                                                                                                "end": 45
                                                                                            },
                                                                                            "initializer": null,
                                                                                            "flags": 32,
                                                                                            "transformFlags": 0,
                                                                                            "start": 39,
                                                                                            "end": 45
                                                                                        }
                                                                                    ],
                                                                                    "trailingComma": false,
                                                                                    "flags": 32,
                                                                                    "transformFlags": 0,
                                                                                    "start": 39,
                                                                                    "end": 45
                                                                                },
                                                                                "flags": 32,
                                                                                "transformFlags": 0,
                                                                                "start": 37,
                                                                                "end": 45
                                                                            }
                                                                        ],
                                                                        "trailingComma": false,
                                                                        "flags": 32,
                                                                        "transformFlags": 0,
                                                                        "start": 37,
                                                                        "end": 45
                                                                    },
                                                                    "contents": {
                                                                        "kind": 216,
                                                                        "functionStatementList": {
                                                                            "kind": 217,
                                                                            "directives": [],
                                                                            "statements": [],
                                                                            "flags": 32,
                                                                            "transformFlags": 0,
                                                                            "start": 45,
                                                                            "end": 45
                                                                        },
                                                                        "flags": 32,
                                                                        "transformFlags": 0,
                                                                        "start": 45,
                                                                        "end": 45
                                                                    },
                                                                    "returnType": null,
                                                                    "flags": 32,
                                                                    "transformFlags": 0,
                                                                    "start": 28,
                                                                    "end": 45
                                                                },
                                                                "argumentList": {
                                                                    "kind": 256,
                                                                    "elements": [],
                                                                    "trailingComma": false,
                                                                    "flags": 32,
                                                                    "transformFlags": 0,
                                                                    "start": 46,
                                                                    "end": 46
                                                                },
                                                                "flags": 32,
                                                                "transformFlags": 1,
                                                                "start": 28,
                                                                "end": 47
                                                            },
                                                            "flags": 16,
                                                            "transformFlags": 4224,
                                                            "start": 24,
                                                            "end": 47
                                                        }
                                                    ],
                                                    "flags": 16,
                                                    "transformFlags": 0,
                                                    "start": 24,
                                                    "end": 47
                                                },
                                                "flags": 16,
                                                "transformFlags": 0,
                                                "start": 20,
                                                "end": 48
                                            }
                                        ],
                                        "flags": 32,
                                        "transformFlags": 0,
                                        "start": 20,
                                        "end": 48
                                    },
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 18,
                                    "end": 50
                                },
                                "flags": 512,
                                "transformFlags": 0,
                                "start": 15,
                                "end": 50
                            },
                            "flags": 512,
                            "transformFlags": 0,
                            "start": 9,
                            "end": 50
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 9,
                    "end": 50
                },
                "flags": 7,
                "transformFlags": 0,
                "start": 32,
                "end": 52
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 52
        }
    ],
    "isModule": false,
    "source": "class C { set x(_) { var f = function { super(); } } }",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 54
}
```

### Printed

```javascript

```

### Diagnostics

```javascript
✖ Missing an opening parentheses - '( - start: 38, end: 39
✖ Object literal keys that are strings or numbers must be a method or have a colon - start: 45, end: 46
✖ ',' expected - start: 45, end: 46
✖ Declaration or statement expected - start: 52, end: 54

```

