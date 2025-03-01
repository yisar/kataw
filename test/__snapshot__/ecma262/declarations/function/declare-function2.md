# Kataw parser test case

## Input

`````js
declare function foo<T>(): void;

declare function foo(x: number, y: string): void;

declare function foo(): void

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
            "kind": 176,
            "declareKeyword": {
                "kind": 82165,
                "flags": 64,
                "transformFlags": 0,
                "start": 0,
                "end": 7
            },
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 7,
                "end": 16
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 16,
                "end": 20
            },
            "typeParameters": {
                "kind": 307,
                "declarations": [
                    {
                        "kind": 146,
                        "name": {
                            "kind": 134299649,
                            "text": "T",
                            "rawText": "T",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 21,
                            "end": 22
                        },
                        "type": null,
                        "assignToken": null,
                        "defaultType": null,
                        "flags": 2097152,
                        "transformFlags": 0,
                        "start": 21,
                        "end": 22
                    }
                ],
                "trailingComma": false,
                "flags": 2097152,
                "transformFlags": 512,
                "start": 21,
                "end": 22
            },
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 24,
                "end": 24
            },
            "contents": null,
            "returnType": {
                "kind": 139,
                "bitwiseOrToken": null,
                "bitwiseAndToken": null,
                "type": {
                    "kind": 138477615,
                    "flags": 2097216,
                    "transformFlags": 0,
                    "start": 26,
                    "end": 31
                },
                "flags": 2097152,
                "transformFlags": 0,
                "start": 26,
                "end": 31
            },
            "flags": 4112,
            "transformFlags": 0,
            "start": 7,
            "end": 31
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 31,
            "end": 32
        },
        {
            "kind": 176,
            "declareKeyword": {
                "kind": 82165,
                "flags": 64,
                "transformFlags": 0,
                "start": 32,
                "end": 41
            },
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 41,
                "end": 50
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 50,
                "end": 54
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [
                    {
                        "kind": 281,
                        "ellipsisToken": null,
                        "left": {
                            "kind": 134299649,
                            "text": "x",
                            "rawText": "x",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 55,
                            "end": 56
                        },
                        "optionalToken": null,
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 134234345,
                                "flags": 2097216,
                                "transformFlags": 0,
                                "start": 57,
                                "end": 64
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 57,
                            "end": 64
                        },
                        "right": null,
                        "flags": 32,
                        "transformFlags": 4096,
                        "start": 55,
                        "end": 64
                    },
                    {
                        "kind": 281,
                        "ellipsisToken": null,
                        "left": {
                            "kind": 134299649,
                            "text": "y",
                            "rawText": "y",
                            "flags": 96,
                            "transformFlags": 0,
                            "start": 65,
                            "end": 67
                        },
                        "optionalToken": null,
                        "type": {
                            "kind": 139,
                            "bitwiseOrToken": null,
                            "bitwiseAndToken": null,
                            "type": {
                                "kind": 134234347,
                                "flags": 2097216,
                                "transformFlags": 0,
                                "start": 68,
                                "end": 75
                            },
                            "flags": 2097152,
                            "transformFlags": 0,
                            "start": 68,
                            "end": 75
                        },
                        "right": null,
                        "flags": 32,
                        "transformFlags": 4096,
                        "start": 65,
                        "end": 75
                    }
                ],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 55,
                "end": 75
            },
            "contents": null,
            "returnType": {
                "kind": 139,
                "bitwiseOrToken": null,
                "bitwiseAndToken": null,
                "type": {
                    "kind": 138477615,
                    "flags": 2097216,
                    "transformFlags": 0,
                    "start": 77,
                    "end": 82
                },
                "flags": 2097152,
                "transformFlags": 0,
                "start": 77,
                "end": 82
            },
            "flags": 4112,
            "transformFlags": 0,
            "start": 41,
            "end": 82
        },
        {
            "kind": 168,
            "flags": 16,
            "transformFlags": 0,
            "start": 82,
            "end": 83
        },
        {
            "kind": 176,
            "declareKeyword": {
                "kind": 82165,
                "flags": 64,
                "transformFlags": 0,
                "start": 83,
                "end": 92
            },
            "asyncKeyword": null,
            "functionKeyword": {
                "kind": 37822554,
                "flags": 64,
                "transformFlags": 0,
                "start": 92,
                "end": 101
            },
            "asteriskToken": null,
            "name": {
                "kind": 134299649,
                "text": "foo",
                "rawText": "foo",
                "flags": 96,
                "transformFlags": 0,
                "start": 101,
                "end": 105
            },
            "typeParameters": null,
            "formalParameterList": {
                "kind": 214,
                "formalParameters": [],
                "trailingComma": false,
                "flags": 32,
                "transformFlags": 0,
                "start": 106,
                "end": 106
            },
            "contents": null,
            "returnType": {
                "kind": 139,
                "bitwiseOrToken": null,
                "bitwiseAndToken": null,
                "type": {
                    "kind": 138477615,
                    "flags": 2097216,
                    "transformFlags": 0,
                    "start": 108,
                    "end": 113
                },
                "flags": 2097152,
                "transformFlags": 0,
                "start": 108,
                "end": 113
            },
            "flags": 4112,
            "transformFlags": 0,
            "start": 92,
            "end": 113
        }
    ],
    "isModule": false,
    "source": "declare function foo<T>(): void;\n\ndeclare function foo(x: number, y: string): void;\n\ndeclare function foo(): void\n",
    "fileName": "__root__",
    "flags": 0,
    "transformFlags": 0,
    "start": 0,
    "end": 114
}
```

### Printed

```javascript
declare function foo(): void;
declare function foo(x: number, y: string): void;

declare function foo(): void;

```

### Diagnostics

```javascript
✔ No errors
```

