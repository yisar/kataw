# Kataw parser test case

## Input

`````js
var C;

function decorator(el) {
  return Object.assign(el, {
    finisher(Class) {
      C = Class;
    },
  });
}

class A {
  @decorator
  foo() {}
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
            "kind": 155,
            "declareKeyword": null,
            "varKeyword": {
                "kind": 37757002,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "declarationList": {
                "kind": 156,
                "declarations": [
                    {
                        "kind": 157,
                        "binding": {
                            "kind": 134299649,
                            "text": "C",
                            "rawText": "C",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 3,
                            "end": 5
                        },
                        "type": null,
                        "initializer": null,
                        "flags": 16,
                        "transformFlags": 4224,
                        "start": 3,
                        "end": 5
                    }
                ],
                "flags": 16,
                "transformFlags": 0,
                "start": 3,
                "end": 5
            },
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 6
        },
        {
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 65,
                "transformFlags": 0,
                "start": 6,
                "end": 16
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "decorator",
                "rawText": "decorator",
                "flags": 96,
                "transformFlags": 0,
                "start": 16,
                "end": 26
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [
                    {
                        "kind": 134299649,
                        "text": "el",
                        "rawText": "el",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 27,
                        "end": 29
                    }
                ],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 27,
                "end": 29
            },
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
                                "flags": 81,
                                "transformFlags": 0,
                                "start": 32,
                                "end": 41
                            },
                            "expression": {
                                "kind": 131,
                                "expression": {
                                    "kind": 129,
                                    "member": {
                                        "kind": 134299649,
                                        "text": "Object",
                                        "rawText": "Object",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 41,
                                        "end": 48
                                    },
                                    "expression": {
                                        "kind": 134299649,
                                        "text": "assign",
                                        "rawText": "assign",
                                        "flags": 96,
                                        "transformFlags": 0,
                                        "start": 49,
                                        "end": 55
                                    },
                                    "flags": 96,
                                    "transformFlags": 2,
                                    "start": 41,
                                    "end": 55
                                },
                                "argumentList": {
                                    "kind": 256,
                                    "elements": [
                                        {
                                            "kind": 134299649,
                                            "text": "el",
                                            "rawText": "el",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 56,
                                            "end": 58
                                        },
                                        {
                                            "kind": 220,
                                            "propertyList": {
                                                "kind": 218,
                                                "properties": [
                                                    {
                                                        "kind": 351,
                                                        "asyncKeyword": null,
                                                        "asteriskToken": null,
                                                        "getKeyword": null,
                                                        "setKeyword": null,
                                                        "method": {
                                                            "kind": 209,
                                                            "name": {
                                                                "kind": 134299649,
                                                                "text": "finisher",
                                                                "rawText": "finisher",
                                                                "flags": 97,
                                                                "transformFlags": 0,
                                                                "start": 61,
                                                                "end": 74
                                                            },
                                                            "typeParameters": null,
                                                            "formalParameterList": {
                                                                "kind": 214,
                                                                "formalParameters": [
                                                                    {
                                                                        "kind": 134299649,
                                                                        "text": "Class",
                                                                        "rawText": "Class",
                                                                        "flags": 96,
                                                                        "transformFlags": 0,
                                                                        "start": 75,
                                                                        "end": 80
                                                                    }
                                                                ],
                                                                "trailingComma": false,
                                                                "flags": 96,
                                                                "transformFlags": 0,
                                                                "start": 75,
                                                                "end": 81
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
                                                                                "kind": 125,
                                                                                "left": {
                                                                                    "kind": 134299649,
                                                                                    "text": "C",
                                                                                    "rawText": "C",
                                                                                    "flags": 97,
                                                                                    "transformFlags": 0,
                                                                                    "start": 83,
                                                                                    "end": 91
                                                                                },
                                                                                "operatorToken": {
                                                                                    "kind": 4125,
                                                                                    "flags": 96,
                                                                                    "transformFlags": 0,
                                                                                    "start": 91,
                                                                                    "end": 93
                                                                                },
                                                                                "right": {
                                                                                    "kind": 134299649,
                                                                                    "text": "Class",
                                                                                    "rawText": "Class",
                                                                                    "flags": 96,
                                                                                    "transformFlags": 0,
                                                                                    "start": 93,
                                                                                    "end": 99
                                                                                },
                                                                                "flags": 0,
                                                                                "transformFlags": 128,
                                                                                "start": 83,
                                                                                "end": 99
                                                                            },
                                                                            "flags": 16,
                                                                            "transformFlags": 4096,
                                                                            "start": 83,
                                                                            "end": 100
                                                                        }
                                                                    ],
                                                                    "flags": 33,
                                                                    "transformFlags": 0,
                                                                    "start": 83,
                                                                    "end": 100
                                                                },
                                                                "flags": 32,
                                                                "transformFlags": 0,
                                                                "start": 81,
                                                                "end": 106
                                                            },
                                                            "flags": 32,
                                                            "transformFlags": 0,
                                                            "start": 74,
                                                            "end": 106
                                                        },
                                                        "flags": 32,
                                                        "transformFlags": 0,
                                                        "start": 61,
                                                        "end": 106
                                                    }
                                                ],
                                                "trailingComma": true,
                                                "flags": 17,
                                                "transformFlags": 0,
                                                "start": 61,
                                                "end": 107
                                            },
                                            "flags": 49,
                                            "transformFlags": 8,
                                            "start": 59,
                                            "end": 111
                                        }
                                    ],
                                    "trailingComma": false,
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 56,
                                    "end": 111
                                },
                                "flags": 32,
                                "transformFlags": 1,
                                "start": 41,
                                "end": 112
                            },
                            "flags": 81,
                            "transformFlags": 256,
                            "start": 32,
                            "end": 113
                        }
                    ],
                    "flags": 33,
                    "transformFlags": 0,
                    "start": 32,
                    "end": 113
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 30,
                "end": 115
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 6,
            "end": 115
        },
        {
            "kind": 178,
            "declareKeyword": null,
            "decorators": null,
            "classKeyword": {
                "kind": 37822544,
                "flags": 81,
                "transformFlags": 0,
                "start": 115,
                "end": 122
            },
            "name": {
                "kind": 134299649,
                "text": "A",
                "rawText": "A",
                "flags": 96,
                "transformFlags": 0,
                "start": 122,
                "end": 124
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
                            "decorators": {
                                "kind": 207,
                                "elements": [
                                    {
                                        "kind": 34611453,
                                        "decoratorToken": {
                                            "kind": 34611453,
                                            "flags": 65,
                                            "transformFlags": 0,
                                            "start": 126,
                                            "end": 130
                                        },
                                        "expression": {
                                            "kind": 134299649,
                                            "text": "decorator",
                                            "rawText": "decorator",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 130,
                                            "end": 139
                                        },
                                        "flags": 0,
                                        "transformFlags": 0,
                                        "start": 130,
                                        "end": 139
                                    }
                                ],
                                "flags": 32,
                                "transformFlags": 0,
                                "start": 126,
                                "end": 139
                            },
                            "staticKeyword": null,
                            "asyncKeyword": null,
                            "setKeyword": null,
                            "getKeyword": null,
                            "asteriskToken": null,
                            "method": {
                                "kind": 209,
                                "name": {
                                    "kind": 134299649,
                                    "text": "foo",
                                    "rawText": "foo",
                                    "flags": 97,
                                    "transformFlags": 0,
                                    "start": 139,
                                    "end": 145
                                },
                                "typeParameters": null,
                                "formalParameterList": {
                                    "kind": 214,
                                    "formalParameters": [],
                                    "trailingComma": false,
                                    "flags": 0,
                                    "transformFlags": 0,
                                    "start": 146,
                                    "end": 147
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
                                        "start": 149,
                                        "end": 149
                                    },
                                    "flags": 32,
                                    "transformFlags": 0,
                                    "start": 147,
                                    "end": 150
                                },
                                "flags": 0,
                                "transformFlags": 0,
                                "start": 145,
                                "end": 150
                            },
                            "flags": 0,
                            "transformFlags": 0,
                            "start": 126,
                            "end": 150
                        }
                    ],
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 126,
                    "end": 150
                },
                "flags": 124,
                "transformFlags": 0,
                "start": 32,
                "end": 152
            },
            "flags": 17,
            "transformFlags": 0,
            "start": 115,
            "end": 152
        }
    ],
    "isModule": false,
    "source": "var C;\n\nfunction decorator(el) {\n  return Object.assign(el, {\n    finisher(Class) {\n      C = Class;\n    },\n  });\n}\n\nclass A {\n  @decorator\n  foo() {}\n}\n",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 153
}
```

### Printed

```javascript
var C;
function decorator(el) {
  return Object.assign(el, {
      finisher(Class) {
        C = Class;
      },
    });
}

class A {
  @decorator foo() {}
}

```

### Diagnostics

```javascript
✔ No errors
```

