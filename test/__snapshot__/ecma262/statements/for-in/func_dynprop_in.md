# Kataw parser test case

## Input

`````js
for (function(){ }[x in y] in x);
`````

## Options

### Parser Options

`````js
{}
`````

### Printer Options

`````js
{
  "tabWidth": 2,
  "printWidth": 80,
  "useTabs": false,
  "bracketSpacing": true
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
            "kind": 166,
            "forKeyword": {
                "kind": 37757017,
                "flags": 80,
                "transformFlags": 0,
                "start": 0,
                "end": 3
            },
            "initializer": {
                "kind": 130,
                "member": {
                    "kind": 177,
                    "asyncKeyword": null,
                    "functionKeyword": {
                        "kind": 37822554,
                        "flags": 64,
                        "transformFlags": 0,
                        "start": 5,
                        "end": 13
                    },
                    "asteriskToken": null,
                    "name": null,
                    "typeParameters": null,
                    "formalParameterList": {
                        "kind": 214,
                        "formalParameters": [],
                        "trailingComma": false,
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 14,
                        "end": 14
                    },
                    "contents": {
                        "kind": 216,
                        "functionStatementList": {
                            "kind": 217,
                            "directives": [],
                            "statements": [],
                            "flags": 32,
                            "transformFlags": 0,
                            "start": 16,
                            "end": 16
                        },
                        "flags": 32,
                        "transformFlags": 0,
                        "start": 15,
                        "end": 18
                    },
                    "returnType": null,
                    "flags": 32,
                    "transformFlags": 0,
                    "start": 5,
                    "end": 18
                },
                "expression": {
                    "kind": 198,
                    "left": {
                        "kind": 134299649,
                        "text": "x",
                        "rawText": "x",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 19,
                        "end": 20
                    },
                    "operatorToken": {
                        "kind": 21006388,
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 20,
                        "end": 23
                    },
                    "right": {
                        "kind": 134299649,
                        "text": "y",
                        "rawText": "y",
                        "flags": 96,
                        "transformFlags": 0,
                        "start": 23,
                        "end": 25
                    },
                    "flags": 96,
                    "transformFlags": 5120,
                    "start": 19,
                    "end": 25
                },
                "flags": 32,
                "transformFlags": 4,
                "start": 5,
                "end": 26
            },
            "inKeyword": {
                "kind": 21006388,
                "flags": 64,
                "transformFlags": 0,
                "start": 26,
                "end": 29
            },
            "expression": {
                "kind": 134299649,
                "text": "x",
                "rawText": "x",
                "flags": 96,
                "transformFlags": 0,
                "start": 29,
                "end": 31
            },
            "statement": {
                "kind": 168,
                "flags": 16,
                "transformFlags": 0,
                "start": 32,
                "end": 33
            },
            "flags": 80,
            "transformFlags": 0,
            "start": 0,
            "end": 33
        }
    ],
    "isModule": false,
    "source": "for (function(){ }[x in y] in x);",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 33
}
```

### Printed

```javascript
for (function () {}[x in y] in x);
```

### Diagnostics

```javascript
✔ No errors
```

