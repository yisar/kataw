# Kataw parser test case

## Input

`````js
function x(){
  if (x) return / /;
  else;
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
            "kind": 176,
            "declareKeyword": null,
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 0,
                "end": 8
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 8,
                "end": 10
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 11,
                "end": 11
            },
            "contents": {
                "kind": 216,
                "functionStatementList": {
                    "kind": 217,
                    "directives": [],
                    "statements": [
                        {
                            "kind": 164,
                            "ifKeyword": {
                                "kind": 37757019,
                                "flags": 81,
                                "transformFlags": 0,
                                "start": 13,
                                "end": 18
                            },
                            "expression": {
                                "kind": 134299649,
                                "text": "x",
                                "rawText": "x",
                                "flags": 96,
                                "transformFlags": 0,
                                "start": 20,
                                "end": 21
                            },
                            "consequent": {
                                "kind": 161,
                                "returnKeyword": {
                                    "kind": 37757022,
                                    "flags": 80,
                                    "transformFlags": 0,
                                    "start": 22,
                                    "end": 29
                                },
                                "expression": {
                                    "kind": 371,
                                    "text": "/ /",
                                    "rawText": "/ /",
                                    "flags": 96,
                                    "transformFlags": 0,
                                    "start": 29,
                                    "end": 33
                                },
                                "flags": 80,
                                "transformFlags": 256,
                                "start": 22,
                                "end": 34
                            },
                            "elseKeyword": {
                                "kind": 4194389,
                                "flags": 65,
                                "transformFlags": 0,
                                "start": 34,
                                "end": 41
                            },
                            "alternate": {
                                "kind": 168,
                                "flags": 16,
                                "transformFlags": 0,
                                "start": 41,
                                "end": 42
                            },
                            "flags": 81,
                            "transformFlags": 0,
                            "start": 13,
                            "end": 42
                        }
                    ],
                    "flags": 33,
                    "transformFlags": 0,
                    "start": 13,
                    "end": 42
                },
                "flags": 32,
                "transformFlags": 0,
                "start": 12,
                "end": 44
            },
            "returnType": null,
            "flags": 16,
            "transformFlags": 0,
            "start": 0,
            "end": 44
        }
    ],
    "isModule": false,
    "source": "function x(){\n  if (x) return / /;\n  else;\n}",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 44
}
```

### Printed

```javascript
function x() {
  if (x) return / /;
  else ;
}
```

### Diagnostics

```javascript
✔ No errors
```

