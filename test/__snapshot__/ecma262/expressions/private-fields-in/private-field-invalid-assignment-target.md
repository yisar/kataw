# Kataw parser test case

## Input

`````js
class C {
  #field;

  constructor() {
    #field in {} = 0;
  }
}
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
                                "text": "#field",
                                "rawText": "#field",
                                "flags": 97,
                                "transformFlags": 0,
                                "start": 9,
                                "end": 18
                            },
                            "optionalToken": null,
                            "type": null,
                            "initializer": null,
                            "flags": 32,
                            "transformFlags": 128,
                            "start": 9,
                            "end": 18
                        },
                        {
                            "kind": 1108353041,
                            "flags": 64,
                            "transformFlags": 0,
                            "start": 18,
                            "end": 19
                        },
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
                                    "flags": 97,
                                    "transformFlags": 0,
                                    "start": 19,
                                    "end": 34
                                },
                                "typeParameters": null,
                                "formalParameterList": {
                                    "kind": 214,
                                    "formalParameters": [],
                                    "trailingComma": false,
                                    "flags": 2048,
                                    "transformFlags": 0,
                                    "start": 35,
                                    "end": 36
                                },
                                "returnType": null,
                                "contents": {
                                    "kind": 216,
                                    "functionStatementList": {
                                        "kind": 217,
                                        "directives": [],
                                        "statements": [
                                            {
                                                "kind": 120,
                                                "expression": {
                                                    "kind": 198,
                                                    "left": {
                                                        "kind": 67191035,
                                                        "text": "#field",
                                                        "rawText": "#field",
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 38,
                                                        "end": 49
                                                    },
                                                    "operatorToken": {
                                                        "kind": 21006388,
                                                        "flags": 96,
                                                        "transformFlags": 0,
                                                        "start": 49,
                                                        "end": 52
                                                    },
                                                    "right": {
                                                        "kind": 125,
                                                        "left": {
                                                            "kind": 220,
                                                            "propertyList": {
                                                                "kind": 218,
                                                                "properties": [],
                                                                "trailingComma": false,
                                                                "flags": 16,
                                                                "transformFlags": 0,
                                                                "start": 54,
                                                                "end": 54
                                                            },
                                                            "flags": 48,
                                                            "transformFlags": 8,
                                                            "start": 52,
                                                            "end": 55
                                                        },
                                                        "operatorToken": {
                                                            "kind": 4125,
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 55,
                                                            "end": 57
                                                        },
                                                        "right": {
                                                            "kind": 201392130,
                                                            "text": 0,
                                                            "rawText": "0",
                                                            "flags": 96,
                                                            "transformFlags": 0,
                                                            "start": 57,
                                                            "end": 59
                                                        },
                                                        "flags": 32,
                                                        "transformFlags": 128,
                                                        "start": 52,
                                                        "end": 59
                                                    },
                                                    "flags": 96,
                                                    "transformFlags": 5120,
                                                    "start": 38,
                                                    "end": 59
                                                },
                                                "flags": 16,
                                                "transformFlags": 4096,
                                                "start": 38,
                                                "end": 60
                                            }
                                        ],
                                        "flags": 33,
                                        "transformFlags": 0,
                                        "start": 38,
                                        "end": 60
                                    },
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 36,
                                    "end": 64
                                },
                                "flags": 2048,
                                "transformFlags": 0,
                                "start": 34,
                                "end": 64
                            },
                            "flags": 2048,
                            "transformFlags": 0,
                            "start": 19,
                            "end": 64
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 9,
                    "end": 64
                },
                "flags": 7,
                "transformFlags": 0,
                "start": 32,
                "end": 66
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 66
        }
    ],
    "isModule": false,
    "source": "class C {\n  #field;\n\n  constructor() {\n    #field in {} = 0;\n  }\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 66
}
```

### Printed

```javascript
class C {
  #field;;
  constructor() {
    #field in {} = 0;
  }
}
```

### Diagnostics

```javascript
✔ No errors
```

