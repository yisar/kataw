# Kataw parser test case

## Options

`````js
{ jsx: false, disableWebCompat: true, module: true }
`````

## Input

`````js
(class { *yield() {} })
`````

## Output

### CST

```javascript
{
    "kind": 122,
    "directives": [],
    "statements": [
        {
            "kind": 120,
            "expression": {
                "kind": 121,
                "expression": {
                    "kind": 189,
                    "decorators": null,
                    "classKeyword": {
                        "kind": 37822544,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 1,
                        "end": 6
                    },
                    "name": null,
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
                                    "getKeyword": null,
                                    "asteriskToken": {
                                        "kind": 201360950,
                                        "flags": 64,
                                        "transformFlags": 32,
                                        "start": 8,
                                        "end": 10
                                    },
                                    "method": {
                                        "kind": 209,
                                        "name": {
                                            "kind": 134299649,
                                            "text": "yield",
                                            "rawText": "yield",
                                            "flags": 96,
                                            "transformFlags": 0,
                                            "start": 10,
                                            "end": 15
                                        },
                                        "typeParameters": null,
                                        "formalParameterList": {
                                            "kind": 214,
                                            "formalParameters": [],
                                            "trailingComma": false,
                                            "flags": 0,
                                            "transformFlags": 0,
                                            "start": 16,
                                            "end": 17
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
                                                "start": 19,
                                                "end": 19
                                            },
                                            "flags": 32,
                                            "transformFlags": 0,
                                            "start": 17,
                                            "end": 20
                                        },
                                        "flags": 0,
                                        "transformFlags": 0,
                                        "start": 15,
                                        "end": 20
                                    },
                                    "flags": 0,
                                    "transformFlags": 0,
                                    "start": 8,
                                    "end": 20
                                }
                            ],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 8,
                            "end": 20
                        },
                        "flags": 6,
                        "transformFlags": 0,
                        "start": 32,
                        "end": 22
                    },
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 1,
                    "end": 22
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 0,
                "end": 23
            },
            "flags": 16,
            "transformFlags": 4096,
            "start": 0,
            "end": 23
        }
    ],
    "isModule": true,
    "source": "(class { *yield() {} })",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 23
}
```

### Printed

```javascript
(class {
    *yield() {}
  });
```

### Diagnostics

```javascript
✔ No errors
```

